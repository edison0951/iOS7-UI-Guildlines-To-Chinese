###Creating Resizable Images

  You can create a resizable image to customize the background of several standard UI elements, such as popovers, buttons, navigation bars, tab bars, and toolbars (including the items on these bars). Providing resizable images for these elements can result in better app performance.

  For many UI elements, you can also specify end caps in addition to a background appearance. An **end cap** defines an area of the image that should not be resized. For example, you might create a resizable image that includes four end caps that define the four corners of a button. When the image is resized to fill the button’s background area, the portions defined by the end caps are drawn unchanged.

  Depending on the dimensions of the resizable image you supply, iOS either stretches or tiles it as appropriate to fill a UI element’s background area. To **stretch** an image means to scale up the image, without regard for its original aspect ratio. Stretching is performant, but it isn’t usually desirable for a multipixel image that can distort. To **tile** an image is to repeat the original image as many times as necessary to fill the target area. Tiling is less performant than stretching, but it's the only way to achieve a textured or patterned effect.

  As a general rule, you should supply the smallest image (excluding end caps) that will result in the look you want. For example:

*   If you want a solid color with no gradient, create a 1 x 1 pixel image.

*   If you want a vertical gradient, create an image that has a width of 1 pixel and a height that matches the height of the UI element’s background.

*   If you want to provide a repeating textured appearance, you need to create an image with dimensions that match the dimensions of the repeating portion of the texture.

*   If you want to provide a nonrepeating textured appearance, you need to create a static image with dimensions that match the dimensions of the UI element’s background area.

		Note
		If you’re creating resizable images to draw on a Retina display, you also need to supply high-resolution versions of your images. For example, you would also supply a solid-color 2 x 2 pixel image, or a gradient image that has a width of 2 pixels.