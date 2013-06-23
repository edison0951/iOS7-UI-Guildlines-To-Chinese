## Launch Image
The launch image is a simple placeholder image that iOS displays when your app starts up. Because the launch image appears so quickly, users get the impression that your app is fast and responsive.

  To enhance the user’s experience at app launch, you must provide at least one launch image.


	Note
	In general, an iPhone app should include a launch image in portrait orientation; an iPad app should include one launch image in portrait orientation and one launch image in landscape orientation.
	
  Because iOS lets you supply different launch images for different usages, you give each image a name that specifies how it should be used. The format of the launch image filename includes modifiers you use to specify the device, resolution, and orientation of the image. To learn how to name launch images appropriately, see [“App Launch (Default) Images”](https://developer.apple.com/library/prerelease/ios/documentation/iPhone/Conceptual/iPhoneOSProgrammingGuide/App-RelatedResources/App-RelatedResources.html#//apple_ref/doc/uid/TP40007072-CH6-SW12) in _[iOS App Programming Guide](https://developer.apple.com/library/prerelease/ios/documentation/iPhone/Conceptual/iPhoneOSProgrammingGuide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40007072)_.

  **Supply a launch image to improve user experience.**

  The launch image isn’t an opportunity to provide:

*   An “app entry experience,” such as a splash screen

*   An About window

*   Branding elements, unless they are a static part of your app’s first screen

  Because users are likely to switch among apps frequently, you should make every effort to cut launch time to a minimum, and you should design a launch image that downplays the experience rather than drawing attention to it.

  **Generally, design a launch image that is identical to the first screen of the app.**

  Exceptions:

  **Text.** The launch image is static, so any text you display in it will not be localized.

  **UI elements that might change.** Avoid including elements that might look different when the app finishes launching, so that users don’t experience a flash between the launch image and the first app screen.

  **For iPhone and iPod touch launch images, include the status bar region.** Create launch images of the following sizes.

  For iPhone 5 and iPod touch (5th generation):

*   640 x 1136 pixels

  For other iPhone and iPod touch devices:

*   640 x 960 pixels

*   320 x 480 pixels (standard resolution)

  **For iPad launch images, don’t include the status bar region.** Create launch images of these sizes (most iPad apps should supply a launch image for each orientation):

*   For portrait:

    *   1536 x 2008 pixels

    *   768 x 1004 pixels (standard resolution)

*   For landscape:

    *   2048 x 1496 pixels

    *   1024 x 748 pixels (standard resolution)

  If you think that following these guidelines will result in a plain, boring launch image, you’re right. Remember, the launch image is not meant to provide an opportunity for artistic expression. It’s solely intended to enhance the user’s perception of your app as quick to launch and immediately ready for use.
