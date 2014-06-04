Mixxx skin snippets for Sublime Text
====================================

This package provides a bunch of handy snippets for doing Mixxx skin development with
[Sublime Text](http://www.sublimetext.com/). It makes inserting widget code in
your Mixxx xml source files easier.

Install
-------

### Git

You can clone [this repository](https://github.com/esbrandt/mixxx-sublime-snippets.git)
into your Sublime Text *Packages* user directory. You really should use
Package Control, though.

#### Mac OS X

    git clone git://github.com/esbrandt/mixxx-sublime-snippets.git ~/Library/Application Support/Sublime Text 3/Packages/User/MixxxSnippets

#### Linux

    git clone git://github.com/esbrandt/mixxx-sublime-snippets.git ~/.config/sublime-text-3/Packages/User/MixxxSnippets

#### Windows

    git clone git://github.com/esbrandt/mixxx-sublime-snippets.git %userprofile%\AppData\Roaming\Sublime Text 3\Packages\User\MixxxSnippets

### Sublime Text - Package Control

**Sorry. Not available in Package Control yet.**

The easiest and best way to manage Sublime Text packages is with
[Package Control][].

1. Install [Package Control][] if you haven't already.
2. Choose *Install Package* from the command palette.
3. Select *Mixxx Snippets* and press Enter.

[Package Control]: http://wbond.net/sublime_packages/package_control

Usage
-----

The snippets will **not** be triggered and automatically added in other types
then xml documents.

So, first apply xml syntax highlighting to your file. In Sublime Text use menu
`View → Syntax → XML`.

### Command palette

![Command palette](https://raw.githubusercontent.com/esbrandt/mixxx-sublime-snippets/master/usage-command-palette.gif)

To insert a snippet in a source file, open the Sublime Text command palette.

    ⌘ + ⇧ + P (Max OSX)
    Ctrl + ⇧ + P (Windows/Linux)

To insert, for example, the Mixxx `<Time>` widget in a source file, open the
command palette, type *Mixxx* and choose *Mixxx -> Time* (or choose *Mixxx ->
Time* from the snippets menu). The code will be inserted at the cursor. The
widgets editable tags details (size, time format, etc.) will be highlighted in
turn so that you can easily tab between them and modify them if necessary.

### Tab trigger

![Tab trigger](https://raw.githubusercontent.com/esbrandt/mixxx-sublime-snippets/master/usage-tab-trigger.gif)

Alternatively, just type the trigger, e.g. `time`, in the xml source file and hit `Tab`.
- Use `TAB` to run a snippet after typing the trigger.
- Use `TAB` and `Shift+TAB` to cycle forward/backward through editable tags.
- Use `ESC` to exit snippet mode.

### Auto completion

In the editor, Sublime Text will show the options as you type (parts of) the trigger keyword. You can insert the snippet by selecting it from the options or completing the trigger keyword and hitting the `Tab` key.

Making sure auto-completion is turned on for xml files.

If auto-completion is not turned on for you, open your personal settings like this:

    Sublime Text 2 > Preferences > Settings - User (Max OSX)
    Preferences > Settings - User (Windows)
    Preferences > Settings - User (Linux)

If you want the autocomplete dropdown to appear in xml files as you type then add this line to your *User Preferences.sublime-settings* file:

    {
        "auto_complete_selector": "text.xml"
    }

Contents - What's included
--------------------------

| Widget name | Description | Tab trigger|
| --- | --- | --- |
| **Buttons** |
||
| **Knobs** |
||
| **Slider** |
| SliderComposed | Display Crossfader  | crossfader |
| SliderComposed | Display Pitch (Speed) fader  | rate |
| SliderComposed | Display channel volume fader  | volume |
| **Text** |
| TextProperty | Display track informations loaded from ID3 the tracks tags | trackproperty |
| NumberBpm | Display current BPM number after speed change | numberbpm |
| NumberBpm | Display numeric volume and gain | numberdb |
| NumberPos | Display playing position / time remaining | numberpos |
| NumberRate | Display pitch (speed) rate | numberrate |
| Key | Display effective musical key | key |
| Label | Display a text label | label |
| Time | Display the current time | time |
| **Layout** |
| Splitter | Control the size of child widgets by dragging the boundary between them | splitter |
| Schemes | Create colored versions of a skin | schemes |
