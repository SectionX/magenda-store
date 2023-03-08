# Magenda Store custom scripts and widgets

    Code to customize magenda-party.myshopify.com e-commerce
    site.

    A collection of html and css styles using liquid as the
    templating language. As a first iteration, the widgets
    will be mostly standalone scripts and markups that I'm 
    planning to eventually turn into layouts.

    This collection is supposed to extend the Dawn theme and
    the plan is to avoid JavaScript as much as possible since
    this is the way Dawn is coded. Also I will avoid using
    other frameworks like bootstrap.

    I will be updating this README as I go, with various
    troubleshoots that I encounter and possible solutions, 
    along with whatever tips and wisdom I gather along the way.


# Tips and Tricks:

    **Upload fonts to Shopify:**

    There is a lot of outdated information about how to do it.
    Assuming you are using the Dawn theme, the steps are as follows:

    1) Download your font. You can use ttf, woff, woff2. Probably more
    but I've tried it with those formats.

    2) Go to admin/content/files and upload the font file.
    !IMPORTANT - Do NOT upload it as an Asset. This is outdated
    and for some reason it doesn't work.

    3) Go to the theme's main liquid file. For Dawn it's
    "theme.liquid". You need to make sure that it's a .liquid
    file and not a .css one.

    4) Inside a {% style %} tag add the following:
    @font-face {
        font-family: "Your font's name";
        src: url {{ "The font's file name" | file_url }} format ("format's name")
    }

    5) The format names are as follows:
        .woff2 -> woff2
        .woff -> woff
        .ttf -> TrueType


# Navigating this repo:

    Each widget has the following files:

    1)  info.md file which provides information, a change
        history and a todo list.

    2)  A static html file with the necessary markup

    3)  An external css file for better readability

    4)  A liquid file that combines both previous 
        files and is ready to be transfered to a 
        "Custom Liquid" section.

    5)  Necessary assets to recreate the final product

    6) There are 2 types of changes. 

        Iterations: Any time I implement something major,
        I will increment the version.
        example: v0.2

        Bug Fixes: I denote bug fixes with letters
        example: v0.2a

        Once the object is ready to enter production,
        it's version will be 1.0. Additional iterations
        will go up to 1.9 and any changes will be applied
        on the live file.

        Once an object enters version 2, the previous file
        will be archived and a new one will take it's place.



# Changes:

    See the respective info.md for changes.

    *Widgets/header-logo: v0.1 (Initial) to v0.2 (2023/7/3)