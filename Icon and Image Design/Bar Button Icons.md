## Bar Button Icons
  iOS defines lots of standard bar-button icons, such as Refresh, Share, Add, and Favorites. If you need to represent custom topics or actions, follow these guidelines to design your own icons.
	  		
<img src="image/bar-icons_2x.png"  width="534" height="54">

  As much as possible, you should use the system-provided buttons and icons to represent standard tasks in your app. For a complete list of standard buttons and icons, and guidelines on how to use them, see [Toolbar and Navigation Bar Buttons](https://developer.apple.com/library/prerelease/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW33) and [Tab Bar Icons](https://developer.apple.com/library/prerelease/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW34).

  Of course, not every task or mode in your app can be represented by a standard icon. As you think about the best way to convey the task or mode, aim for a design that is:

*   **Simple and streamlined.** Too many details can make an icon appear sloppy or indecipherable.

*   **Not easily mistaken for one of the system-provided icons.** Users should be able to distinguish your custom icon from the standard icons at a glance.

*   **Readily understood and widely acceptable.** Strive to create a symbol that most users will interpret correctly and that no users will find offensive.

		Important
		Be sure to avoid using images that replicate Apple products in your designs. These symbols are copyrighted and product designs can change frequently.

  A custom icon that you provide for a toolbar, navigation bar, or tab bar is also known as a **template** image, because iOS uses it as a mask to create the icon you see in your app. If you ceate a full-color template image, iOS ignores the color.

  After you’ve decided on the appearance of your icon, follow these guidelines as you create it:

*   Use pure white with appropriate alpha transparency.

*   Don’t include a drop shadow.

*   Use anti-aliasing.

*   If you decide to add a bevel, be sure that it’s 90° (to help you do this, imagine a light source positioned at the top of the icon).

  For  toolbar and navigation bar icons on iPhone, iPod touch, and iPad, create an icon in the following sizes:

*   About 44 x 44 pixels

*   About 22 x 22 pixels (standard resolution)

  For tab bar icons on iPhone, iPod touch, and iPad, create an icon in the following sizes:

*   About 60 x 60 pixels (96 x 64 pixels maximum)

*   About 30 x 30 pixels (48 x 32 pixels maximum) for standard resolution

  Don’t include text in a custom tab bar icon. Instead, use the tab bar item APIs to set the title for each tab (for example, ["initWithTitle:image:tag:"](https://developer.apple.com/library/prerelease/ios/documentation/UIKit/Reference/UITabBarItem_Class/Reference/Reference.html#//apple_ref/occ/instm/UITabBarItem/initWithTitle:image:tag:)). If you need to adjust the automatic layout of the title, you can use the title adjustment APIs (such as ["setTitlePositionAdjustment:"](https://developer.apple.com/library/prerelease/ios/documentation/UIKit/Reference/UITabBarItem_Class/Reference/Reference.html#//apple_ref/occ/instm/UITabBarItem/setTitlePositionAdjustment:)).
  
		Note
		For a tab bar icon, you can also provide a set of two fixed images, one for the unselected appearance and one for the selected appearance.

  **Give all icons in a bar a similar visual weight.** Aim to balance the overall size, level of detail, and use of solid regions across all icons that can appear in a specific bar. In general, it doesn’t look good to combine in the same bar icons that are large and blocky, and completely filled, with icons that are small, detailed, and unfilled.
