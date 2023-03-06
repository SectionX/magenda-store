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
