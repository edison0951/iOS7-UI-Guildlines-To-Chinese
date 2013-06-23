## Icon and Image Sizes
Every app needs an app icon and a launch image. In addition, some apps need custom icons to represent app-specific content, functions, or modes in navigation bars, toolbars, and tab bars.

Unlike other custom artwork in your app, the icons and images listed in <span class="x-name-no-link">Table 38-1</span> must meet specific criteria so that iOS can display them properly. In addition, some icon and image files have naming requirements. (If you need to support standard-resolution iPhone or iPod touch devices, divide by 2 the high-resolution sizes listed below.)

  <table class="graybox" border="0" cellspacing="0" cellpadding="5">
    <caption class="tablecaption"> **Table 38-1** Size (in pixels) of custom icons and images</caption>
    <thead>
        <tr>
            <th scope="col" class="TableHeading_TableRow_TableCell">   -
  Description

</th>
            <th scope="col" class="TableHeading_TableRow_TableCell">

  Size for iPhone 5 and iPod touch (high resolution)

</th>
            <th scope="col" class="TableHeading_TableRow_TableCell">

  Size for iPhone and iPod touch (high resolution)

</th>
            <th scope="col" class="TableHeading_TableRow_TableCell">

  Size for iPad (high resolution)

</th>
            <th scope="col" class="TableHeading_TableRow_TableCell">

  Size for iPad 2 and iPad mini (standard resolution)

</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td scope="row">
-  ----

App Icon (**required** for all

</td>
            <td>

  apps)|120

</td>
            <td>

  x 120|120

</td>
            <td>

  x 120|144

</td>
            <td>

  x 144|72 x 
</td>
        </tr>
        <tr>
            <td scope="row">
7  2

App Icon for the App Store (**required** for all apps)

</td>
            <td>

  1024 x 1024

</td>
            <td>

  1024 x 1024

</td>
            <td>

  1024 x 1024

</td>
            <td>

  1024 x 1024

</td>
        </tr>
        <tr>
            <td scope="row">

  Launch image (**required** for all apps)

</td>
            <td>

  640 x 1136

</td>
            <td>

  640 x 960

</td>
            <td>

  1536 x 2048 (portrait)

  2048 x 1536 (landscape)

</td>
            <td>

  768 x 1024 (portrait)

  1024 x 768 (landscape)

</td>
        </tr>
        <tr>
            <td scope="row">

  Small icon for Spotlight search results (recommended)

</td>
            <td>

  80 x 80

</td>
            <td>

  80 x 80

</td>
            <td>

  80 x 80

</td>
            <td>

  40 x 40

</td>
        </tr>
        <tr>
            <td scope="row">

  Small icon for Settings (recommended)

</td>
            <td>

  58 x 58

</td>
            <td>

  58 x 58

</td>
            <td>

  58 x 58

</td>
            <td>

  29 x 29

</td>
        </tr>
        <tr>
            <td scope="row">

  Toolbar and navigation bar icon (optional)

</td>
            <td>

  About 44 x 44

</td>
            <td>

  About 44 x 44

</td>
            <td>

  About 44 x 44

</td>
            <td>

  About 22 x 22

</td>
        </tr>
        <tr>
            <td scope="row">

  Tab bar icon (optional)

</td>
            <td>

  About 60 x 60 (maximum: 96 x 64)

</td>
            <td>

  About 60 x 60 (maximum: 96 x 64)

</td>
            <td>

  About 60 x 60 (maximum: 96 x 64)

</td>
            <td>

  About 30 x 30 (maximum: 48 x 32)

</td>
        </tr>
        <tr>
            <td scope="row">

  Default Newsstand cover icon for the App Store (**required** for Newsstand apps)

</td>
            <td>

  At least 1024 pixels on the longest edge

</td>
            <td>

  At least 1024 pixels on the longest edge

</td>
            <td>

  At least 1024 pixels on the longest edge

</td>
            <td>

  At least 1024 pixels on the longest edge

</td>
        </tr>
        <tr>
            <td scope="row">

  Web clip icon (recommended for web apps and websites)

</td>
            <td>

  120 x 120

</td>
            <td>

  120 x 120

</td>
            <td>

  144 x 144

</td>
            <td>

  72 x 72

</td>
        </tr>
    </tbody>
  </table>
  For all images and icons, the PNG format is recommended. You should avoid using interlaced PNGs.

  The standard bit depth for icons and images is 24 bits—that is, 8 bits each for red, green, and blue—plus an 8-bit alpha channel.

  You don’t need to constrain your palette to web-safe colors. 