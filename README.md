Rainbow
=======

Rainbow is a CSS library for pretty, colorful buttons. It comes with sources written in both Sass and LESS for easy customization. No dependencies on any other third party library.

To see the buttons, open example.html in your browser or check out [the demo page](http://projects.cristanradu.com/rainbow/).

Rainbow is licensed [Creative Commons CC-BY](http://creativecommons.org/licenses/by/3.0/), which means you can freely share and/or modify it for both personal and commercial applications. The only requirement is that you keep the original attribution (the comment at the top of the CSS file).

The basic button style is based on the [Apple OS X Lion Buttons in CSS](http://pixify.com/blog/use-os-x-lion-to-improve-your-ui/) by Pixify.


Basic Usage
-----------

If you want to use the library as-is, with just the default buttons (showcased on [the demo page](http://projects.cristanradu.com/rainbow/) then all you need is the CSS file. Include it in your header: 

    <link rel="stylesheet" type="text/css" href="css/rainbow.css" media="screen">

To create a basic button, all you need to do is use the base rainbow class (.rb):

    <a class="rb">Button</a>

The library includes a few additional styles: selected, disabled, small and grouped buttons. You get 12 colors included by default, listed below. For a colorful button, include the base class and the desired color: 

    <a class="rb rb-blue">Blue Button</a>


Custom Colors
-------------

If you'd like more customization - including defining your own colors - then download the full archive. You'll find inside both Sass and LESS source files that can be imported into your own stylesheets. Use whichever one you prefer.

In your project's Sass/LESS stylesheet, add the following import at the top:

    @import 'rainbow';

Since you're importing Rainbow into your own stylesheet, you no longer need to include its CSS file in your header (as in the basic use example above). Get rid of it.

Define your own selector and call the rainbow-button mixin with your custom color:

    // Sass
    .rb-lightblue { @include rainbow-button(#e6eaf6); }

    // LESS
    .rb-lightblue { .rainbow-button(#e6eaf6); }

Build the stylesheet and you're good to go. Now you can use your custom color from the compiled CSS:

    <a class="rb rb-lightblue">Custom Button</a>

That's it! Enjoy using Rainbow! 