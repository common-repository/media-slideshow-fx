=== Media Slideshow FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, media, slideshow, free, flash, as3, xml, autoplay, images, videos, playlist, transitions, effects, text, css
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

An original Media Slideshow. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. It supports images (JPG, BMP, PNG, GIF), videos and SWFs with customizable widths and heights for the whole application. The playlist position and orientation is customizable and has roll over/out effects. The text is HTML/CSS formatted and can be placed on playlist and over the images. It also has autoplay functionality and a lot of other customizable properties on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/media-slideshow-fx.zip "Media Slideshow FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/media-slideshow.zip "Media Slideshow FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **media-slideshow-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Media Slideshow FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[media-slideshow-fx][/media-slideshow-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Media Slideshow FX part of your theme, edit the template files and add `<?php mediaslideshowfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Media Slideshow FX](http://www.flashxml.net/media-slideshow.html "Media Slideshow FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/media-slideshow-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/media-slideshow-fx/images/` and update the `wp-content/flashxml/media-slideshow-fx/images/thumbs.xml` and `wp-content/flashxml/media-slideshow-fx/images/big.xml` files accordingly

= Additional settings file =

To embed the Media Slideshow FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[media-slideshow-fx settings="settings2.xml"][/media-slideshow-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `mediaslideshowfx_echo_embed_code()` function call (for example `<?php mediaslideshowfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[media-slideshow-fx]` and `[/media-slideshow-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `mediaslideshowfx_echo_embed_code()` function call (for example `<?php mediaslideshowfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[media-slideshow-fx width="600" height="300"][/media-slideshow-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `mediaslideshowfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/media-slideshow.html "Media Slideshow FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/media-slideshow-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/media-slideshow.html "Media Slideshow FX") is the utility that helps easily customize your Media Slideshow FX to fit all your needs.