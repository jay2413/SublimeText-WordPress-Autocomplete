## WordPress Sublime Text 2

This adds autocomplete for WordPress Functions, Hooks, Constants and Classes for Sublime Text 2

### Notes

The other WordPress sublime package was not up to date and missing stuff so I build a custom parser for grabbing data from WP core.

    Current WP version : 3.6
     
    Functions  : 3165
    Hooks      : 1544
    Constants   :  121
    Classes    :   74


Deprecated functions have been removed :smiley_cat:  

Many hooks/functions are duplicated throughout the WP code-base (contain different parameters), so it is necessarily to tab through the options for some autocompletes.

Hooks names which start as a variable have been removed, for example `do_action($page_hook)`, there are not many of these in WP and there is no great way to add them to Sublime.

*There might be some slight issues with hook completions due them being inconsistently named by WP, still testing this plugin*


### Tip

Sublime won't autocomplete PHP files when there is no closing `?>` tags , so in "Preferences-->Settings-User" add this snippet:

    "auto_complete_selector": "source, text",

### ToDo

Add some useful snippets


#### Manual
  
Download the .zip or git clone this into your sublime packages location, you can find it under "Preferences-->Browse Packages".

