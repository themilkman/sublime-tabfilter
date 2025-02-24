# Tab Filter

Tab Filter is a Sublime Text plugin for quickly switching between open tabs.  Invoking Tab Filter brings up a "GoTo Anything"-like quick input showing your opened tabs for the current window, allowing you to quick filter on file names to rapidly switch amongst existing tabs.

## Compatibility

This plugin is compatible with Sublime Text 3 and 4 (and still should be with 2).

## Installation

### Package Control

Tab Filter is also available through [Package Control](http://wbond.net/sublime\_packages/package\_control).  To install, bring up the Command Palette (brought up using `ctrl+shift+p` on Linux / Windows or `cmd+shift+p` on OS X) and run the `Package Control: Install Package` command - now search for and select **Tab Filter**.

### Manual

From within Sublime Text, go to the `Preferences` > `Browse Pacakges` menu; this should open up your file browser at the correct location for where your copy of Sublime text stores all packages.

From within this folder you can install...

#### Using git

You can install within the Packages folder opened by running the following from a terminal / console:

    $ git clone git://github.com/robinmalburn/sublime-tabfilter.git 'Tab Filter'

#### Without git

To install without git, download the source code as a zip file and extract the contents to into a subfolder of the Packages folder called `Tab Filter`

## Usage

### Key Bindings

Tab Filter comes with the following default keymap for Linux, OSX and Windows:  `alt+shift+p`

This can be overriden via the keybindings options in `Preferences > Package Settings > Tab Filter > Key Bindings - User`

### Command Palette

Tab Filter can also be activated via the Command Palette (brought up using `ctrl+shift+p` on Linux / Windows or `cmd+shift+p` on OS X) and typing Tab Filter

### Settings

Additional configuration settings for Tab Filter can be altered via `Preferences > Package Settings > Tab Filter > Settings - User`

##### Captions

Tab Filter can be configured to show or hide additional captions relating to the state of each open tab.  The captions include: *Current File*, *Unsaved File*, *Unsaved Changes* and *Read Only*.  Captions are shown by default, but this behaviour can be changed by setting the `show_captions` setting to `false`.

##### Path/Filename Filtering

By default, Tab Filter only shows the basename of open tabs (where they're really files and not just buffers, of course).  This configuration can be changed to instead show and therefore allow filtering by the full, non-common path of the file instead by changing the `include_path` option to `true`.

##### Preview currently selected entry

By default, Tab Filter only focuses the tab if it gets selected. To always focus/preview the currently highlighted entry, set `preview_tab` to `true`. Note that this currently only works with a single group layout (no splitted window).


## License

Released under [MIT license](https://github.com/robinmalburn/sublime-tabfilter/blob/master/license.txt).