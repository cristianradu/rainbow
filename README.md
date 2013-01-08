Rainbow
=======

Rainbow is a set of colorful CSS3 buttons written in Sass. The button styles are based on the [Apple OS X Lion Buttons in CSS](http://pixify.com/blog/use-os-x-lion-to-improve-your-ui/) by Pixify.

Basic Usage
-----------

Download the archive and uncompress it or clone the repository. For a quick, out-of-the box use, just include the compiled CSS file:

    <link rel="stylesheet" type="text/css" href="css/rainbow.css" media="screen">

To create a basic button, all you need to do is use the base rainbow class (rb):

    <a class="rb">Button</a>

You get 12 colors included by default: red, orange, yellow, green, blue, purple, pink, and extras: lime, mint, aqua, cobalt, rose. For a colored button, include the base class and the desired color:

    <a class="rb rb-blue">Blue Button</a>

There are additional styles: selected, disabled, small and grouped buttons. Open up example.html in your browser for a showcase of all possibilities.

Custom Colors
-------------

In order to add custom colors, you need to edit the source Sass file. You could also try to edit the CSS file directly, but you'd have to calculate all the background gradients yourself. Yeah, I didn't think so either.

Add your color as a variable (it'll only be used once - in the selector - but this way we keep the file clean):

    $color-lightblue: #e6eaf6;

Then, at the bottom, create a selector for it by calling the rainbow-button mixin:

    .rb-lightblue { @include rainbow-button($color-lightblue); }

Build the Sass file and that's it! Now you can use your custom color from the CSS:

    <a class="rb rb-lightblue">Custom Button</a>

Enjoy!
