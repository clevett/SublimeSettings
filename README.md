# SublimeSettings
Sublime HTML/JavaScript Syntax for Editing Roll20 sheets 

## How to use
1. In Sublime text go to Preferences -> Browse Packages...
2. Create a new folder called HTML(Unsure how important the foldername is)
3. Copy the two files into the folder
4. Add this Readme as a .yaml as well if you want to access it more easily

(This is supposed to overrule the default settings the files with the same name contains, without editing them directly. )

## Features

Original settings by *Cassie* made html files to also display JavaScript higlight that often can be found on roll20 html files. This fork is an attempt to include a few tweaks that can come handy when working on editing Roll20 character sheets.


### i18n-data html attribute highlight

The `i18n-data` html attribute is changed to be highlighed in orange instead of the default green for attributes. The attributes value is highlighed in blue. Handy if you're in progress of creating/editing language tags for sheets
![data-i18n attribute](/images/data-i18n.png)

### custom html tag highlights

The HTML tags `button`,`rolltemplate` and `charactermancer` are changed to show up in orange instead of the default red for html tags

![button](/images/button.png)

## Making changes

I've included **some** comments in the html syntax file that should help in editing it. If you want to disable a specific highlight, `Ctrl`+`F` throught the file for instances that are specific. 

## Emmet

Emmet is a package that can speed up writing code, and you can easily add your own abbrevations/snippets for it. When you write the keyword and press tab, Sublime's Emmet package will autocomplete to the corresponding code snippet. I've added the following abbrevations that I felt are useful:

* `datas` becomes `<span data-i18n=""></span>`
* `char` becomes `<charmancer></charmancer>`
* `butt` becomes `<button type=\"roll\" name=\"roll_\"></button>`
* `attr` becomes `<input type=\"text\" name=\"attr_\" value=\"\">`

Reading the guide I made:
* `data` becomes `data": "data-i18n=""` as a snippet, instead of an abbreviation, as the documentation suggested it behaved slightly differently

I also added `rolltemplate` and `charmancer` as recognized `html` tags but it didn't seem to work.
