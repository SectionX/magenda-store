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