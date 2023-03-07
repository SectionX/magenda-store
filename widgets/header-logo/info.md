v0.2
# Changes

* Added the file in Magenda's Dawn's library.
* Added media queries. Site supports 360px width as the smallest screen
* Updated Liquid and used native language to include CSS
* Added a skeleton schema with a "presets" field
* Updated container classes for better management
* Linked the Oregano font from Google Fonts
* Added the font to Shopify's backend (theme.liquid file)
* Finished the smartphone layout
* Added fixed sizes for better loading on mobiles

# Todo

1) Test and decide on different layouts for desktop and tablet.
2) Explore the possibility of adding a search field on wider screens.
3) Unlink Google Fonts and use Shopify Fonts instead for better latency.
4) Fix the bug that clips a few pixels from the top of the logo
   // This bug happens only on shopify.
5) Decide on the layout for desktops and tables and implement the media query.
6) Create dynamic color rules

# Completed Todos
1) Test different sizes and fonts for the motto - Completed

   Decided on Oregano font and 23px size for the motto. 

2) Include the motto in the theme's translations - Subverted
   and make it dynamic 

   I decided to leave it hardcoded. The motto isn't
   supposed to be localized anyway.

3, 4 -> Transfered to next iteration


v0.1
# Todo

1) Test different sizes and fonts for the motto
2) Include the motto in the theme's translations
   and make it dynamic
3) Decide on the layout for desktops and tables
   and implement the media query.
4) Create dynamic color rules

# General info

The html and css are the static source files.

The liquid file takes the 2 static files,
combines them and injects dynamic elements.

dynamic elements:
1) Logo -> {{ "Logo-test.jpg" | file_url }}
