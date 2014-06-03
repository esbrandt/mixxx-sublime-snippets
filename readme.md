Mixxx skin snippets for Sublime Text
====================================

This package provides a bunch of handy snippets for doing Mixxx skin development with
[Sublime Text](http://www.sublimetext.com/). It makes inserting widget code in
your Mixxx xml source files easier.

### Installation

##### Git

You can clone [this repository](https://github.com/esbrandt/mixxx-sublime-snippets.git)
into your Sublime Text *Packages* user directory. You really should use
Package Control, though.

##### Package Control
**Sorry. Not available in Package Control yet.**
The easiest and best way to manage Sublime Text packages is with
[Package Control][].

1. Install [Package Control][] if you haven't already.
2. Choose *Install Package* from the command palette.
3. Select *Mixxx Snippets* and press Enter.

[Package Control]: http://wbond.net/sublime_packages/package_control

Install
-------

### Mac OS X

    git clone git://github.com/esbrandt/mixxx-sublime-snippets.git ~/Library/Application Support/Sublime Text 3/Packages/User/MixxxSnippets


### Linux

    git clone git://github.com/esbrandt/mixxx-sublime-snippets.git ~/.config/sublime-text-3/Packages/User/MixxxSnippets


### Windows

    git clone git://github.com/esbrandt/mixxx-sublime-snippets.git %userprofile%\AppData\Roaming\Sublime Text 3\Packages\User\MixxxSnippets

### Sublime Text - Package Control

Install via package control: http://wbond.net/sublime_packages/community
Search for **Mixxx Snippets** or typically the keywords **Mixxx** is suitable.

### Usage

To insert a snippet in a source file, open the Sublime Text command palette.
	* `⌘ + ⇧ + P` (Max OSX)
	* `Ctrl + ⇧ + P` (Windows/Linux)

To insert, for example, the Mixxx <Time> widget in a source file, open the
command palette, type *Mixxx* and choose *Mixxx ->: Time* (or choose *Mixxx ->:
Time* from the snippets menu). The code will be inserted at the cursor. The
widgets editable tags details (size, time format, etc.) will be highlighted in
turn so that you can easily tab between them and modify them if necessary.

ALternatively, just type the trigger in the source file and hit `Tab`.
- Use `TAB` to run a snippet after typing the trigger, e.g. `time,tab`.
- Use `TAB` and `Shift+TAB` to cycle forward/backward through fields.
- Use `ESC` to exit snippet mode.
