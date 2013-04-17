=== WP Supersized ===
Contributors: worldinmyeyes
Donate link: http://www.worldinmyeyes.be/donate/
Tags: Supersized, background, full screen, slideshow, flickr, Picasa, Smugmug, media gallery, NextGEN gallery
Requires at least: 3.1
Tested up to: 3.5
Stable tag: 3.1.5
License: GPLv2

Full screen background slideshow in any page/post, with images from WP Media Gallery, NextGEN Gallery, Flickr, Picasa, Smugmug, folder, or XML file

== Description ==

WP Supersized allows you to display a resizable full screen background slideshow on pages/posts of your choice.
After activation you will find a new WP Supersized section in your Settings where you can manage the plugin options.
A WP Supersized panel will also be available in the post/page editor to select the source of images used by the plugin individually for the current post/page.

*Users may use images from NextGEN Gallery, the Wordpress Media Gallery, Flickr, Picasa, Smugmug, their own choice of directory within the wp-content folder, or a list of slides defined in an xml file (for advanded users).*

WP Supersized integrates the Supersized jquery extension in the pages/posts of your choice. I am not the developer of the original Supersized jquery extension itself, [Supersized](http://buildinternet.com/project/supersized/ "Supersized webpage") was written by [Sam Dunn](http://vivalasam.com/ "Sam Dunn"). My plugin only integrates it into your theme and gives you easy access to many options for displaying this resizeable slideshow background where you want on your website or blog.

So, what exactly does WP Supersized do?

*   Cycles Images/backgrounds via slideshow with transitions and preloading (use it as background or as slideshow)
*   Resizes images to fill browser while maintaining image dimension ratio
*   Navigation controls with keyboard support
*   Integration with NextGEN Gallery and with the Wordpress Media Gallery - choose images from NextGEN galleries or attached to post/page
*   Integration with Flickr - pull photos by user, set, tag, or group
*   Integration with Picasa - pull photos by album, user,or tag
*   Integration with Smugmug - pull photos by keyword, user, gallery, category
*   Accepts jpg, gif, and png images
*   Simple selection of your images source for each page/post separately (also options for advanced users, using an XML file)
*   HTML and links can be used within the images captions (when using WP Media Gallery, NextGEN Gallery, or an XML file as source of images).

You can see an example of Supersized in use in a Wordpress page on the [WP Supersized page](http://www.worldinmyeyes.be/2265/ "WP Supersized page") or on my [About page](http://www.worldinmyeyes.be/about-2/ "About page").
For more details about Supersized itself and its development, check [Supersized](http://www.buildinternet.com/project/supersized/ "the Supersized website").

WP Supersized allows you to display Supersized on the pages/posts that you want in your current theme. Many options are available to choose where and how it will be displayed.

= Options =

There is a number of available options, shown below with their default values. *Not every option is functional in the Single image mode*.
WP Supersized also adds an additional option tab in the page/post editor for easy selection of the source of images for each post/page individually. A source selected on an individual page/post will override the general options choice. When no value has been set for these options yet, they use the general options.

*Functionality*

* *Type of background*

Determines which type of slideshow will be used.

Slideshow: The images that you have uploaded to your `/wp-content/supersized-slides/` directory or the ones attached to the post/page through the Wordpress Media Gallery (have a look at the FAQ to find out how this works) will be shown.

Single image: A single image will be used (the first one found in the slides folder if you have more than one). Slideshow controls will not appear in this mode.

Flickr images: Images will be pulled from Flickr (by user, set, group, or tags see the Flickr options below). If you choose this, please be aware that not all Components options and none of the Supersized Shutter theme specific options will be available with the current version of Supersized.

* *Autoplay on/off*

Determines whether the slideshow begins playing automatically when the page is loaded.

* *Start on slide #*

The slide the slideshow starts on (default is 1). Slides are sorted in alphabetical order of their filename.
In the Single image mode, it controls which image is loaded, 0 causes a random image to be loaded each time (assuming that you have several images in the `/wp-content/supersized-slides/` directory).

* *Random slides*

When on, slides are shown in a random order and the starting slide number will be disregarded. Default is off.

* *Slide interval*

Time between slide changes in milliseconds. The default is 3 seconds.

* *Transition*

Controls which effect is used to transition between slides. Options are as follows:

    No transition effect
    Fade effect (Default)
    Slide in from top
    Slide in from right
    Slide in from bottom
    Slide in from left
    Carousel from right to left
    Carousel from left to right

* *Speed of transition*

The time transitions take in milliseconds (default is 500 milliseconds).

* *New window*

Whether or not slide links open in a new window (default is on).

* *Pause on hover*

Pauses the slideshow when the current image is hovered over. If navigation is enabled, the pause button will become active to show paused state. Disabled by default.

* *Stop loop*

Pauses the slideshow upon reaching the last slide (default is off).

* *Keyboard navigation*

Keyboard navigation (default is on).
Spacebar pauses, Up/Right go to next slide, and Down/Left go to previous slide.

* *Performance*

Uses image rendering options in Firefox and Internet Explorer to adjust image quality. This can speed up/slow down transitions. Webkit does not yet support these options.

    Normal - No adjustments
    Hybrid Speed/Quality - Lowers image quality during transitions and restores after completed (Default)
    Optimizes image quality
    Optimizes transition speed - Faster transition speed, lower image quality

* *Image protection*

Disables right clicking and image dragging using Javascript (default is off).

* *Background URL*

Type here the URL of the link you want to access when clicking on the background image (www.example.com). The same link will be used for all images. Leave this field empty if your do not want any link to be used. Default is empty.

*Display*

* *Select the page(s) where Supersized should be used*

Choose where you want to apply Supersized. These are the most general options. More precise selections are possible below.

    Everywhere (except admin pages)
    All pages (except homepage)
    Homepage (of your blog)
    Front page (landing page)
    Error page (404)
    Search results page
    All posts (not pages)
    Sticky post
    Category archive
    Tag archive
    Date archive
    Any archive
From version 2.0, the option `Only on posts/pages with custom field SupersizedDir` has been removed. Any page/post that has an image source other than `none` will display Supersized.
If you select All posts, All pages, or Everywhere, posts/pages with an image source other than `none` will show images from the corresponding folder while all others will show the default directory images.
In each of these options, unless a specific image source was defined in the page/post, the default slides directory will be used.

* *Select the page template(s) where Supersized should be used*

This option lists all available custom templates in the current theme. You may select one or several of them.
The list is empty if your current theme does not use any custom template.
Please reset the options when you change theme to make sure that the list is updated.

* *Post ID where Supersized will be used*

Type here a comma-separated list of the post IDs where you want Supersized to appear.
Don't forget to deselect `All posts` or `Sticky post` above.
You can find your post IDs in the Posts admin menu by hovering on the name of the post. The ID will be displayed at the bottom of your browser. Alternatively, you can use the [WP Show IDs](http://wordpress.org/extend/plugins/wp-show-ids/ "WP Show IDs ( simple, yet elegant )") plugin.

* *Page ID where Supersized will be used*

Type here a comma-separated list of the page IDs where you want Supersized to appear.
Don't forget to deselect `All pages`, `Homepage`, `Front page`, or `Error page` above.
You can find your page IDs in the Pages admin menu by hovering on the name of the page. The ID will be displayed at the bottom of your browser. Alternatively, you can use the [WP Show IDs](http://wordpress.org/extend/plugins/wp-show-ids/ "WP Show IDs ( simple, yet elegant )") plugin.

* *Category ID for the posts/pages where Supersized will be used*

Type here a comma-separated list of the category IDs where you want Supersized to appear.
You can find your Category IDs in the Posts > Categories admin menu by hovering on the name of the category. The ID will be displayed at the bottom of your browser. Alternatively, you can use the [WP Show IDs](http://wordpress.org/extend/plugins/wp-show-ids/ "WP Show IDs ( simple, yet elegant )") plugin.

* *Tag ID for the posts/pages where Supersized will be used*

Type here a comma-separated list of the tag IDs where you want Supersized to appear.
You can find your Tag IDs in the Posts > Post Tags admin menu by hovering on the name of the tag. The ID will be displayed at the bottom of your browser. Alternatively, you can use the [WP Show IDs](http://wordpress.org/extend/plugins/wp-show-ids/ "WP Show IDs ( simple, yet elegant )") plugin.

*Slides source*

* *Default slides directory*

Select here the slides directory that will be used by default (default is supersized-slides if it exists). Only folders are shown by the selector. Some folders such as `plugins`, `themes`, `cache`, and a few others are not shown by the selector.
The images from the selected directory will be displayed by Supersized unless you use a custom directory in each post/page.
Please put your images folders (default or custom) for Supersized in your `wp-content` directory. You may create folders within folders, e.g. `/wp-content/supersized-slides/slidesforpost###/`.
*If you have been using the `SupersizedDir` custom field in your pages/posts, it is still used but is now shown and selected with a selector. You do not need to fill the custom field yourself anymore.*
WP Supersized will look first for a custom images source that you would have set up for the current page/post. If not found, it will then use the default directory selected here (do not forget to create it and fill it with images!). If none of these can be found, the default Supersized images will be shown.

* *Debugging mode on/off*

When on, WP Supersized will generate comments in the source of the web page (in the slides list) with some variables and arrays values, useful to find out the origin of file path problems. If you have problems with displaying your images, send me these comments from the source of the page and I will be able to help you more easily.
This is not necessary for normal operation. Use only if you have trouble with displaying your images.
(default is off)

*Size and position*

* *Minimum width allowed, Minimum height allowed*

Minimum dimensions the image is allowed to be. If either is met, the image won't size down further (default is 0).

* *Center the background vertically*

Centers image vertically. When turned off, the images resize/display from the top of the page (default is on).

* *Center the background horizontally*

Centers image horizontally. When turned off, the images resize/display from the left of the page (default is on).

* *Always fit*

Prevents the image from ever being cropped. Ignores minimum width and height. (default is off).

* *Fit portrait*

Prevents the image from being cropped by locking it at 100% height (default is on).
This will usually cause vertical images to not cover the window entirely.

* *Fit landscape*

Prevents the image from being cropped by locking it at 100% width (default is off).
This will usually cause horizontal images to not cover the window entirely.

*Components*

**The following options are not taken into account when in Single image mode.**

* *Navigation arrows*

Displays arrows for navigation (default is on).

* *Slideshow controls*

Turns the navigation on/off (default is on).
When turned off, the whole Supersized footer is hidden and the navigation controls are hidden. You may still display the captions (if the `Slides captions` option is on) even when this option is turned off. This allows the use of html in captions without the Supersized footer being displayed.
When turned off, the controls will not be visible but the keyboard navigation will still be available (unless you disable it in the corresponding option).
For custom navigation buttons, replace the images in your `/wp-content/plugins/wp-supersized/img/` folder.

* *Thumbnail navigation*

Toggles forward/backward thumbnail navigation (default is off). When on, thumbnails from the next/previous posts are generated and can be clicked to navigate. If there is no thumbnail available for the slide, it will simply scale down the full size image, which can slow performance.
For both Thumbnail navigation and Thumbnail links in thumbnail tray, thumbnail files must be present in a `thumbs/` directory within the corresponding slides folder, each thumbnails having the same name (+ suffix) as its corresponding image, i.e. the slide `image_1.jpg` in `wp-content/supersized-slides` and its thumbnail `image_1-1.jpg` in `wp/content/supersized-slides/thumbs`.
Thumbnails must be 150 px high to avoid resizing by Supersized.

* *Thumbnail suffix*

The suffix to use for recognizing the thumbnails. Default is -1.

* *Thumbnail tray*

Thumbnail tray appears at the bottom of the screen when clicked on bottom right arrow (default is on).
If you select this option and do not select the next one, there will be no thumbnail in the tray which is not really useful.
See the `Thumbnail navigation` option above for details about thumbnails.

* *Thumbnail links in thumbnail tray*

 Generates a list of thumb links in the thumbnail tray that jumps to the corresponding slide. If there is no thumbnail available for the slide, it will simply scale down the full size image, which can slow performance (default is on)

* *Slide links*

    None
    Numbers
    Slide title
    Empty (default)

Shows a list of the slides in the navigation bar - Better to leave it on `Empty` or `None` for now, as there are still some issues with how Supersized is displaying this.

* *Slide numbers*

Enables/Disables the slide counter (default is on).

* *Slide caption*

Enables/Disables slide captions (default is on).
According to the source of images, captions are extracted from:

* The `IPTC caption` field of the jpg image file for default or custom folders
* The `caption field` of the image for WP Gallery images.
* The `description field` of the image for NextGEN gallery images.
* The `title field` of the corresponding image in the xml file.

* *Progress bar*

Enables/Disables the progress bar shown at the bottom of the screen (default is on).

* *Fluid thumbnail bar*

Enables/Disables the fluid move of the thumbnail bar to the left or right based on mouse location (default is off).

*Flickr*

**The following options are specific to the Flickr mode.**

* *Flickr Source*

Tells Supersized which of the options to pull the images from.

Set: pulls images from a set.

User: pulls images from a user.

Group: pulls images from a group (default).

Tags: pulls images by tags.

* *Set*

You must provide the ID number of the desired set (located in the URL).

* *User*

You must provide the ID number of the desired user ([idgettr.com](http://idgettr.com/ "idgettr.com")).

* *Group*

You must provide the ID number of the desired group ([idgettr.com](http://idgettr.com/ "idgettr.com"))

* *Tags*

You must provide the desired tag(s)

* *How many pictures to pull*

Between 1-500 (default is 100).

* *Flickr Size*

The image size to pull - t,s,m,z,b (smallest to largest, default is z).
Details on [flickr.com](http://www.flickr.com/services/api/misc.urls.html "flickr.com")

* *Sort Images By*

Sort images by date posted, date taken, or interestingness (Default is Date posted).

* *Sort Direction*

Select the sort direction (Default is Descending).

* *Flickr API key*

You need this in order for this to work. You need to get your own at [flickr.com](http://www.flickr.com/services/apps/create/ "flickr.com")

*Picasa*

**The following options are specific to the Picasa mode.**

* *Picasa Source*

Tells Supersized which of the options to pull the images from.

Album : pulls images from a Picasa album (default).

User: pulls images from a user.

Tags: pulls images by tag.

* *Album*

You must provide the ID of the desired album. It can be found in the URL of the link to this album.

* *User*

You must provide the ID number of the desired user (either you Picasa user name or the long number in the URL to your profile).

* *Tags*

You must provide the desired tag(s). You may combine several tags (comma- or "+"-separated = AND, "|"-separated = OR).

* *How many pictures to pull*

Between 1-500 (default is 100).

* *Picasa Image Size*

The image size to pull - 512, 640, 720, 800, 1024, 1280, 1440, 1600. The Picasa API will return the largest size available if your selection is larger than the original.

* *Sort Images By*

Sort images by date published or date updated (none uses default Picasa order) (Default is Date published).

* *Sort Direction*

Select the sort direction (Default is Descending).

* *Picasa Author key*

You need this in order for private albums to work. It can be found in the URL of the link to a private album (each album has a different author key)

*Smugmug*

**The following options are specific to the Smugmug mode.**

* *Smugmug Source*

Tells Supersized which of the options to pull the images from.

Keyword: pulls images by keyword.

User: pulls images from a user.

Gallery: pulls images from a gallery.

Category: pulls images by category.

* *Keyword*

Comma-separated Smugmug keywords (they are combined).

* *User*

You must provide the nickname of the desired user. You may combine it with keyword(s).

* *Gallery*

You must provide the ID of the desired gallery

* *Category*

You must provide the desired category.

* *How many pictures to pull*

Between 1-100 (default is 100). This is currently the maximum allowed by the Google Feed API used by the plugin to get the images.

* *Smugmug Size*

The image size to pull - Tiny, Thumb, Small, Medium, Large, XLarge, X2Large, X3Large, Original.
Details on [help.smugmug.com](http://help.smugmug.com/customer/portal/articles/93250 "smugmug.com")

* *Sort Images By*

Sort images by date published or date updated (none uses default Smugmug order) (Default is Date posted).

* *Sort Direction*

Select the sort direction (Default is Descending).

* *Update*

Click here and your options will updated!

* *Reset*

To reset all WP Supersized options.
*Required when you change theme.*

== Installation ==

1. Download the WP Supersized zip file and unzip it.
2. Upload the WP Supersized folder to your `/wp-content/plugins/` directory. Alternatively, use the Wordpress plugin install in `Plugins >> Add New >> Upload` to upload and install the zip file.
3. Activate the plugin through the `Plugins` menu in WordPress.
4. If you wish to use your own folder containing images, create a `supersized-slides` directory within your wp-content directory. This will be the default folder where images should be uploaded for WP Supersized.
5. If you prefer not to use a folder as described in steps 4, you may use the images attached to a post/page with the Wordpress Media Gallery or NextGEN Gallery, or images from Flickr, Picasa, or Smugmug instead.
7. Go to the `Settings >> WP Supersized` menu and modify the options as desired. The source of images can also be defined independently for each post/page in the post/page editor.

== Frequently Asked Questions ==

= How do I display Wordpress Media Library images with Supersized ? =
 
Simply attach images from the Wordpress Media Library to your new post or page. You do not need to insert them in the post/page, only attach them.
The images will be shown by Supersized in the menu order. So moving them up or down the list in the Media Gallery menu will have the effect of changing their order when displayed by WP Supersized.
WP Supersized will use the caption defined in the Media Gallery. If it is not present, it will use the image title (filename).
To let WP Supersized know that it should display the images from the Media Gallery, select WP Gallery in the Supersized meta box (below the editor) in the page/post editor.
If you have used the `SupersizedDir` custom field before, do not worry, your data is not lost; it is simply shown in an easier way. You do not need to fill in the custom field yourself anymore.
Posts or pages using the Media Gallery images will all use the options defined in the plugin admin.

= How do I display NextGEN Gallery images with Supersized ? =
 
Simply use NextGEN Gallery as you would normally to define galleries.
The images will be shown by Supersized in the order that you chose in NextGEN. So moving them up or down the list in the NextGEN Gallery menu will have the effect of changing their order when displayed by WP Supersized.
For the caption, WP Supersized will use the Description field that you defined in your NextGEN gallery. If it is not present, it will use the image Alt&Title field, also defined in NextGEN.
To let WP Supersized know that it should display the images from the NextGEN Gallery, select NextGEN Gallery in the Supersized meta box (below the editor) in the page/post editor.
To select the NextGEN gallery that you want to use on this page/post, choose it in the WP Supersized panel or in the plugin options.
Posts or pages using the NextGEN Gallery images will all use the options defined in the plugin options.

= What should I do to use a different images folder for each post/page ? =

There are several ways to do it:

* Use the WP Media Gallery (see above)
* Use the NextGEN Gallery (see above)
* Use an XML file (see below) to define your list of images
	
Alternatively, you may create folders containing images for specific pages/folders:
1. Create a folder that will contain your images in your wp-content folder, e.g. the folder `/wp-content/images_for_post_1` will contain the images for a particular post. It is also possible to create folders inside folders, e.g. `/wp-content/images/images_for_page_x`.
2. Once the folder(s) created, add the desired images there.
3. In the post/page editor, select the folder that you want to use from the list displayed in the Supersized meta box below the editing window (only folders are displayed).

= How do I set up different options on each page/post for choosing how to display Supersized and which images it uses ? =

From version 2.0, WP Supersized allows advanced users to choose almost all options *separately for each page/post*, including:

* Almost all options available in the plugin options.
* The list of slides to use (URL).
* The list of thumbnails to use (URL).
* The caption (title) to use for each slide. HTML and links can also be used within this caption.
* The link (URL) where the user will be directed when clicking on the image background (individually for each image).

Details of how to use the XML file can be found in the `example.xml` file provided in the WP Supersized plugin folder. Simply make a copy of this file in your `wp-content` directory or another location within this directory, rename it, and edit it as you wish.

To use an XML file, go to the page/post editor and select the option in the page/post Supersized meta box below the editing window. You also need to enter the path inside the `wp-content` directory and the name of the XML file in the `XML file` field.
*IMPORTANT: if you use xml files for defining your images, two slides field names must be renamed from version 3.0: `slide-link` to `slide_link` and `slide-thumb` to `slide_thumb` in the xml files*.

For example, if you want to use an xml file containing specific options and/or slides for a particular page/post, let's suppose that you have copied the `example.xml` file and created a file called `my_slides_list_and_options.xml` in directory `wp-content/my_wpsupersized_slides_definitions` (choose the names as you wish).
You would then need to enter `my_wpsupersized_slides_definitions/my_slides_list_and_options.xml` in the Supersized meta box below the editing window.
That's all, WP Supersized will now use your own definitions of the slides/options on this particular page/post.

WP Supersized will use default options (as defined in the plugin admin) for any options not defined in the XML files.
Similarly, if you do not define any slides within your XML file, the default directory slides (usually in the `supersized-slides` directory) will be used.

= WP Supersized is installed and activated, my slides folder contains images, and I have set up the options to show Supersized. Why is the Supersized slideshow still not visible ? =
 
In order to see the slideshow, you must make sure that the background of the current page/post is at least partly transparent or leaves some transparent space around it.
If you want your page/post to appear over a semi-transparent background that lets the Supersized slideshow visible, you should modify the css of your template(s).
Here is a useful [link showing the css](http://perishablepress.com/press/2009/01/27/cross-browser-transparency-via-css/ "cross-browser transparent background") needed for a cross-browser transparent background.

= How can I have links in the captions of the images ? =

This is not available for the default or custom folders as captions for images from these are extracted from the IPTC caption field of the file.
You have several possibilities to have links in the captions:

* If you use the WP gallery, you can simply type html code (including links) in the `caption field` of the images. It will then be displayed automatically by WP Supersized.
* If you use the NextGEN gallery, same principle but you need to type it in the `description field`.
* The last way to do it is to use an xml file (as explained in the FAQ and in the example.xml file). There, you can put html code in the `title field`

= Why does Supersized not work with Internet Explorer 6 ? =

Sam Dunn has made the choice not to support IE6 anymore. If you are still using IE6, you should seriously think about upgrading!

= Supersized does not resize the images correctly in Internet Explorer =

Although it seems to appear only sporadically, this was a known bug of Supersized 3.1.x. The latest version of Supersized (from 3.2.4) used in this plugin should solve this issue but is not yet available for the flickr mode.

= Why are images not resized to full screen on iPads or some Android tablets ? =

It has been reported that Supersized images are not resized correctly on iPad and Android tablets. As far as I know, this is mostly due to the way they are handling images and their interpretation of some css. There is currently no clear solution for this.

= What are the image formats that can be used with Supersized ? =

Since version 1.2 of WP Supersized, the following formats are recognized: jpg, jpeg, gif, png.

= Why are only default images or an image indicating an error displayed when my Wordpress installation has its own folder ? =

If you see an image indicating an error, it should point you to one of the possible causes for this problem.
First of all, make sure to update to the latest version of the plugin.
If the issue is still present, there is probably a problem with file access permissions on your server. This has mostly been observed when running servers based on Windows. Try changing access rights to your image folder to solve this.
It could also be that your provider has disabled the glob() function in php. Some providers seem to have done this to avoid a security issue with glob() in versions of php earlier than 5.2.4. It is not necessary anymore from php version 5.2.4 and higher so there should be no reason to leave the glob() function disabled. If you are in this case, contact your provider and ask them to enable the glob() function. Thanks to Sandro for finding out about this.

= Where is the SupersizedDir custom field ? =

*THIS IS NOT NEEDED ANYMORE FROM VERSION 3.0 BUT IS LEFT HERE FOR YOUR INFORMATION*

At the bottom of the page/post you are creating/editing, you should see a box called Custom Field. If it is not visible, go to Screen Options (top right of the page) and check Custom Field.
In the Custom Field box, enter the new Custom Field name *SupersizedDir* (next time, it will appear automatically in the list of Custom Field names).
According to what you want to do, you can then give it a value that is the name of the folder to use for this particular post/page, or the value `wp-gallery` to use the Wordpress Media Gallery, or (for advanced users) the location of an xml file containing all slides, titles, links, and options for this particular page/post.

== Screenshots ==

1. Page/post specific options - You may choose the source of images for each post/page independently.
2. General options/Functionality - Define the behaviour of Supersized.
3. General options/Display - Choose where Supersized will be displayed.
4. General options/Slides source - Choose which images source should be used as default.
5. General options/Size and position - Choose how the images will be displayed.
6. General options/Components - Fine-tune the navigation controls for Supersized.
7. General options/Flickr - Enter here the details of your Flickr account and the choice of Flickr images.
8. General options/Picasa - Enter here the details of your Picasa account and the choice of Picasa images.
9. General options/Smugmug - Enter here the details of your Smugmug account and the choice of Smugmug images.
10. Example of selection of images in the post editor (individual selection for each post/page).


== Other notes ==

= Thanks =

A big Thank You to Sam Dunn for developing the Supersized jquery extension.

Thanks to the many developers who make so much information available for those (like me) who need to learn from more experienced people.

Special thanks to Joke and Sandro who helped me finding the solution to a bug present in the plugin when Wordpress is installed in its own folder.

Thanks to the generous donators who encourage me to develop my plugin further (and start working on new ones!) by [making a donation](http://www.worldinmyeyes.be/donate/ "Donate").

== Changelog ==

= 3.1.5 =

* Added the option Always fill screen in Size and position, to allow the image to always fill the screen (image is cropped). This possibility had disappeared when the new Size and position button was introduced in v.3.1.2.

= 3.1.4 =

* Bug fix (tested): corrected several errors in the automatic options conversion routine that were still preventing the plugin to work correctly.
This bug fix will only work on new updates from versions before v.3.1.2.
If you were faced with problems when updating to v.3.1.2 or v.3.1.3, the solution is to take a note of your current options and then to reset the options and enter your own options again. Sorry for the inconvenience.

= 3.1.3 =

* Bug fix: added more checks in the automatic options conversion routine to avoid the issue of losing the options when updating. This bug fix will only work on new updates from versions earlier than v.3.1.2.
If you were faced with the problem when updating to v.3.1.2, the solution is to take a note of your current options and then to reset the options and enter your own options again. Sorry for the inconvenience.

= 3.1.2 =

* Bug fix: fixed a small syntax error in jquery code used by the plugin that was causing problems with the display of the backend metabox in WP 3.5.
* Bug fix: the options selected through an xml file should now work as advertised.
* Bug fix: the thumb tray will now appear only when the corresponding option (Thumbnail tray) is selected, even if the option for showing the tray at startup is selected.
* Bug fix: modified the Flickr, Picasa, and Smugmug code used by the plugin to avoid the disappearance of the navigation arrows when a long caption is displayed.
* Bug fix: the Fit always option should now work also with Flickr, Picasa, and Smugmug images.
* Modified the Size and position option: Fit always, Fit portrait, and Fit landscape are now mutually exclusive. There was no point in selecting both Fit portrait and Fit landscape at the same time to do what Fit always does anyway.
* Added support for displaying the Supersized source meta box in custom post types (thanks to [JonasVorwerk](http://wordpress.org/support/profile/jonasvorwerk "JonasVorwerk")).
* Added enhanced jquery animate to remove flickering on iPad and iPhone ([jquery.animate-enhanced plugin](http://playground.benbarnett.net/jquery-animate-enhanced/ "jquery.animate-enhanced plugin")).
* Added more details for the use of some options in the admin.
* Added an automatic option updater to set the right format for the on/off options.
* Updated the example.xml file with the missing options for Picasa, and Smugmug.
* Cleaned up some code.
* Tested up to WP 3.5.

= 3.1.1 =

* Bug fix: moved a few lines in their correct position in the code. This small mistake was generating warnings about invalid arguments passed to the implode() function.
* Bug fix: added a few additional checks in the admin to avoid warnings about invalid arguments passed to the implode() function.
* Bug fix: rewrote the install() function to remove errors introduced in version 3.1.
* Eliminated a few php notices (undefined index).
* Cleaned up some html in the admin of the plugin.

= 3.1 =

* Added support for the use of images from Picasa and Smugmug.
* Added the ability to sort Flickr images (thanks to [mendhak](https://github.com/mendhak "mendhak")).
* Now with easy individual selection of source (WP Media Gallery, NextGen Gallery, Flickr, Picasa, Smugmug, custom dir, or XML file) for each page/post.
* Bug fix: Removed a trailing slash in the function listing the folders and files. This was causing an open_basedir restriction error in php versions older than 5.2.2.
* Bug fix: The image source selected within a post/page is now used even when the Flickr or Single modes are defined as default in the plugin options.
* Bug fix: The debugging mode will not break the page anymore. Debugging info now appears correctly as a comment in the page source.
* Bug fix for square photos in Flickr module (thanks to [Matt Richardson](https://github.com/matt-richardson "Matt Richardson")).
* Added a jquery.easing.compatibility.js file to help solving issues that appeared for some users (thanks to [Twanneman](http://twanneman.nl/) "Twanneman").
* Improved: Navigation arrows will not be displayed anymore when there is only one image to show. Thanks to [Artem](http://wordpress.org/support/profile/artemkolotilkin "Artem") and [Glark](http://wordpress.org/support/profile/glark "Glark") for noticing this issue and hacking a solution while I was updating the plugin.
* Modified the plugin files structure to improve modularity.
* Cleaned up the code of the install function.
* Updated the readme.

= 3.0.2 =

* Added an option to display the thumbtray at startup to avoid having to click on the button to show it.
* Bug fix: added typecasting to the array_merge() function.
* Improvement: now also checking that the NextGEN Gallery plugin is active (on top of checking for its presence).
* Updated the readme.

= 3.0.1 =

* Bug fix: the plugin should now work as expected on some configurations where the backend was screwed up due to a wrong function call.
* Bug fix: re-enabled the previous glob() function (on top of the new one) to allow for different configurations, some of them missing their images.

= 3.0 =

* Added support for the use of images from NextGEN galleries.
* Added a panel in post/page editor to allow the selection of the images source - *no need to type your selection in a custom field anymore*.
* Redesigned the options panel, using tabs to reduce clutter.
* Added a folder selector to the options page for easy selection of the default folder or NextGEN gallery.
* Added the ability to have captions displayed even if the rest of the Supersized footer is off (allows displaying html from image caption even with the footer option off).
* Added checks for the existence and read permissions for image folders and NextGEN or WP Media gallery images - displays an informative error image if an error is detected.
* Updated with the latest versions of Supersized (3.2.7) and its Shutter theme (1.2).
* Improved: the glob() function should now work better for users with some servers that do not support the BRACE option. Thanks to Jan for suggesting this.
* Improved: replaced the url by the absolute path for reading xml files to avoid possible problems with some hosts. Thanks to [Aaron Ware](http://wordpress.org/support/profile/aware/ "Aaron") for suggesting this.
* Improved: automatic removal of slashes in the default dir and custom dir paths.
* Bug fix: archive, tag, category, or date pages should now correctly display the default images.
* Bug fix: the plugin should now work correctly with xml files containing no images: default images are shown instead (as advertised!).
* Bug fix: the plugin should now work correctly with IE when using WP Gallery images. Thanks to [Simon](http://profiles.wordpress.org/users/lumpysimon/ "Simon") for spotting this bug.
* Updated the readme.
* Removed the xmlLib library. The plugin now uses standard SimpleXML functions. *IMPORTANT: if you use xml files for defining your images, two slides field names must be renamed: `slide-link` to `slide_link` and `slide-thumb` to `slide_thumb` in the xml files*.

= 2.0 =

* Added the ability to use the Wordpress Media Gallery images attached to pages/posts as source of images.
* Added the ability to use an xml file to define all images, titles, links, and options for each post/page separately.
* Added the ability to use HTML and links in the caption of the images (only when using the xml file).
* Behaviour change: slight modification to allow an image to be displayed even when there is only one in the chosen folder and in slideshow mode.
* Behaviour change: removed the option `Only on posts/pages with custom field SupersizedDir`. Any post/page that has a custom field SupersizedDir filled in will use Supersized.
* Bug fix: the navigation controls are now working as expected in the Flickr mode.

= 1.5.1 =

* Bug fix: WP Supersized now works correctly with WPML-translated pages/posts (caution: not tested if you use a different domain per language).
* Added a donation link in the plugin admin.

= 1.5 =

* Bug fix: modified the way the plugin finds the slides folder so that it finally works with non-standard Wordpress installations (e.g. when Wordpress has its own folder). Special thanks to Joke and Sandro who helped me finding the solution to this bug by testing several beta versions on their system.
* Bug fix: the play/pause buttons behave correctly again (a previously corrected bug had been reintroduced when updating to Supersized 3.2.6).

= 1.4 =

* Updated with the latest version of Supersized (3.2.6).

= 1.3 =

* Added the option to output a few comments in the source of the web page to help in debugging the problems that some users have with the file path to their images folders.
* Bug fix: filenames are now always sorted alphabetically in the slides list output.

= 1.2.2 =

* Bug fix: fixed a bug in the Single image mode that prevented the image to be displayed.

= 1.2.1 =

* Bug fix: fixed a bug that caused an error when there was no thumbs folder.

= 1.2 =

* Updated with the latest version of Supersized (3.2.5).
* Bug fix: fixed a bug that prevented images to be displayed correctly when in Tag or Category results page.
* Bug fix: fixed a bug that prevented Supersized to be used in subcategories of a chosen category.
* Bug fix: WP Supersized should now take into account the location of the wp-content folder also in non-standard Wordpress installations.
* Added the ability to use gif and png image formats in addition to jpg (can now also be jpeg).
* Added the options to use Supersized everywhere, on Search results page only, on Date archives, or on Any archive.
* Added the option to have a URL of your choice when clicked on the background image (one for all images), or none.

= 1.1.1 =
* Updated with the latest modified Supersized Flickr engine, including the option to choose images by tags.
* Bug fix: the Flickr slideshow broken with the previous update now works again.

= 1.1 =
* Updated with the latest version of Supersized (3.2.4).
* The `slides` folder must now be renamed `supersized-slides` and be placed in the `/wp-content` directory instead of the `/wp-content/plugins/wp-supersized` directory. This allows updates without losing your images.
* Added the ability to choose any folder within the `/wp-content` folder as a default slides folder.
* Added the ability to select a different slides folder for each page/post through the custom field `SupersizedDir`.
* Added more options for selecting the pages/posts where Supersized will be used: Category archive, Tag archive, Category ID, Tag ID.
* Bug fix: Random image now works as expected in Single image mode.
* Bug fix: the loader image (progress.gif) now loads and displays correctly. 
* Added new Supersized options.
* Admin page ready for translation (.pot file available). Anyone interested in translating WP Supersized in his/her own language ?
* Added French translation. 
* Removed the Supersized logo option (not present in the original Supersized example anymore).

= 1.0 =
* The very first version.

== Upgrade Notice ==

Bug fix (working this time!) to avoid the loss of options experienced by users who updated to v.3.1.2 and v.3.1.3. This bug fix will only work on new updates from versions before v.3.1.2.
If you were faced with the problem when updating to v.3.1.2 or v.3.1.3, the solution is to take a note of your current options and then to reset the options and enter your own options again. Sorry for the inconvenience.