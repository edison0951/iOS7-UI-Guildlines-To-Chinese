## Newsstand Icon
  If your app uses Newsstand Kit to publish subscription-based periodical content, you need to provide icons for display in the App Store and on people’s devices.

<image src="image/mag-news-temp.png"/>

	Important
	The aspect ratio of all Newsstand icons should be between 1:2 and 2:1. 	All Newsstand icons must be flat and have 90° corners.
	Don’t add perspective to any of your Newsstand icons.

  All Newsstand apps need to supply a Newsstand cover icon that represents the default cover art in the App Store. The long edge of this icon should measure at least 1024 pixels (512 pixels for standard-resolution devices). Note that this icon is separate from the app icon that all iOS apps must provide.

A default Newsstand cover icon should be a generalized facsimile of the cover of a typical issue, which focuses on the parts of the cover that are fairly consistent from issue to issue. For example:

*   Avoid adding to the default cover icon elements that users would never see on an actual cover, such as a message to “tap here for the latest issue”.

*   Avoid using artwork or headlines that are seasonal or topical, such as images related to holidays or headlines that refer to current events.

  In particular, don’t reuse the cover of a previous issue for your default Newsstand cover icon, because users might confuse your app with a specific issue.

  In addition to the default Newsstand cover icon, you also need to supply a separate icon that accurately represents each new issue so  it can appear on the Newsstand shelf and in the multitasking UI on an iOS device. Unlike the default cover icon, each per-issue icon should display details about the contents of a specific issue. 

  It’s recommended that you create a single large icon for each issue, and allow iOS to scale it for display in both places (the icon displayed in Newsstand is larger than the icon displayed in the multitasking UI). Depending on the precise location of an issue on a Newsstand shelf, iOS might also add perspective to the icon so that it matches the realistic look of the shelf.

  Specifically, you should create a per-issue icon whose long edge measures at least 1024 pixels (512 pixels for standard-resolution devices). To display the current issue’s icon on the Newsstand shelf and in the multitasking UI, iOS scales your large icon to the following sizes:

  **Table 42-1** Maximum scaled sizes for the long edges of per-issue icons

Device|Scaled long-edge size (Newsstand shelf)|Scaled long-edge size (multitasking UI)
:-----------:  | :----------- |  :-----------
iPhone and iPod touch|180 pixels (90 pixels for standard resolution)|114 pixels (57 pixels for standard resolution)
iPad|252 pixels (126 pixels for standard resolution)|144 pixels (72 pixels for standard resolution)

  In addition to providing icons, you use keys in your app’s `Info.plist` file to define how the icons should appear on iOS devices. 

*   First, use the binding type key to indicate whether your content is a magazine or a newspaper.

*   Then, use the binding edge key to specify the visual enhancements that iOS should add to the icon, such as the fold at the bottom edge of a standard newspaper.

  For more information about these keys and their values, see [“Contents of the UINewsstandIcon Dictionary”](https://developer.apple.com/library/prerelease/ios/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html#//apple_ref/doc/uid/TP40009249-SW15) in _[Information Property List Key Reference](https://developer.apple.com/library/prerelease/ios/documentation/General/Reference/InfoPlistKeyReference/Introduction/Introduction.html#//apple_ref/doc/uid/TP40009247)_.

  When you specify the magazine binding type, iOS adds the appearance of multiple pages and a shadow that suggests thickness. You must also specify a left or right binding edge for a magazine icon, to indicate the edge that should receive the stapled binding appearance.

  For example, suppose that you supply a per-issue icon similar to this:

<image src="image/magazine_before.jpg"/>

  If you specify the left binding edge, iOS adds the stapled binding appearance to the left edge and the multiple-page appearance to the right edge.

<image src="image/magazine_after.jpg"/>

  When you specify the newspaper binding type, iOS adds the appearance of additional copies of the paper that are stacked beneath the current issue. 

  If your newspaper is standard size, you can specify a bottom binding edge to give your icon the appearance of a fold at its bottom edge. If your newspaper is tabloid-size—that is, approximately half the size of a broadsheet—you can specify left, right, or no binding edge to avoid the addition of the fold appearance.

  For example, suppose that your per-issue newspaper icon looks similar to this:

<image src="image/newspaper_before.jpg" />

  If you specify the bottom binding edge, iOS adds the appearance of a fold to the bottom edge. (iOS adds the stacked-paper appearance regardless of the value you supply for the binding edge key.)

<image src="image/newspaper_after.jpg" />

  For additional information about setting up a Newsstand app, see _[iTunes Connect Developer Guide](https://developer.apple.com/library/prerelease/ios/documentation/LanguagesUtilities/Conceptual/iTunesConnect_Guide/1_Introduction/Introduction.html#//apple_ref/doc/uid/TP40011225)_.