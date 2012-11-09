# My Sublime Text 2 Settings

## Requirements:

- [Sublime Text 2][]
- [Package Control][]
- [Ubuntu Mono][] font

## Installation

### Using Git

Install [Ubuntu Mono][] font, then [Sublime Text 2][], open up ST2, enter license, install [Package Control][], quit ST2.

Go to your Sublime Text 2 Packages directory:

    cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/

Remove default `User` folder:

    rm -rf User

Clone the settings repository using the command below:

    git clone https://github.com/lars-feyerabend/st2-user-settings.git "User"

Or, if you are me:

    git clone git@github.com:lars-feyerabend/st2-user-settings.git "User"

Done. Now open ST2 again and wait for Package Control to download the configured 
packages. You might want to check the console (Ctrl-`) for output.

## Preferences Overview

I have to do this here, since ST2 keeps removing comments from the Settings file.

### Appearance

    "theme": "Soda Light.sublime-theme",
    "color_scheme": "Packages/Tomorrow Color Schemes/Tomorrow-Night.tmTheme",
    "font_face": "Ubuntu Mono",
    "font_options":
    [
      "subpixel_antialias"
    ],
    "font_size": 16,
    "line_padding_bottom": 1,
    "line_padding_top": 1

I really like the [Soda Light][] look for UI, coupled with [Tomorrow Night][]
for syntax highlighting. And recently, I've switched to [Ubuntu Mono][] instead
of [Consolas][], my previous favorite programming font. I add a little padding
to make it easier on the eye.

    "highlight_line": true

Helps me see where I am.

    "highlight_modified_tabs": true

Blue dot instead of gray dot. I like it.

    "rulers": [80]

I like to keep my code lines within 80 characters, so I don't go insane if I
have to edit a file remotely on a terminal.



### Behavior

    "create_window_at_startup": true

No empty window on startup. I'll open one if I need one.

    "drag_text": false

For me, text dragging only ever happens accidentally and is hard to catch and
recover from if not immediately noticed.

    "find_selected_text": true

Sounds reasonable.

    "show_tab_close_buttons": false

Prevent accidental closing.


### File Handling

    "tab_size": 2

Two spaces is plenty for indentation.

    "ensure_newline_at_eof_on_save": true

Mostly [historic][] reasons, but I consider it good style.

    "translate_tabs_to_spaces": true

I use spaces for a consistent style. Tabs visually break indentations when
set to a different width.

    "trim_trailing_white_space_on_save": true

Ugh, I *hate* trailing white space.

    "ignored_packages":
    [
      "Vintage"
    ]

Go home, Vim. This is 2012.

[Sublime Text 2]: http://www.sublimetext.com/
[Package Control]: http://wbond.net/sublime_packages/package_control
[Soda Light]: https://github.com/buymeasoda/soda-theme
[Consolas]: http://www.microsoft.com/en-us/download/details.aspx?id=17879
[Tomorrow Night]: https://github.com/chriskempson/tomorrow-theme
[Ubuntu Mono]: http://font.ubuntu.com/
[historic]: http://stackoverflow.com/questions/729692/why-should-files-end-with-a-newline
