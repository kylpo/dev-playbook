# Apps
- [Anbox \- Android in a Box](https://anbox.io/) - Run Android applications on Linux
  - [Anbox Installation, Setup, and Test \- Run Android Applications on Linux\! \- YouTube](https://www.youtube.com/watch?v=Or9uzQLb3ws)
- [autokey](https://github.com/autokey/autokey) - for scripting and key remapping
  - More on this later
- [Pithos – Pandora Radio Client](https://pithos.github.io/)
- [Spotify for Linux](https://www.spotify.com/us/download/linux/)

# Gnome-Shell
Gnome Shell is the future of Ubuntu, so let's embrace it! I am currently using the [Ubuntu GNOME](https://wiki.ubuntu.com/UbuntuGNOME/GetUbuntuGNOME) distro.

## Customizations
- [AlternateTab](https://extensions.gnome.org/extension/15/alternatetab/) for an alt-tab that does NOT group by application (similar to Window's alt-tab)
  - I choose to enable `Show only windows in the current workspace`
- [AppMenu Window Title](https://extensions.gnome.org/extension/743/appmenu-window-title/) - shows the current focused window's title in menubar
- [Applications Menu](https://extensions.gnome.org/extension/6/applications-menu/) - for an app launcher when you're in Mouse-mode
  - ![](https://extensions.gnome.org/extension-data/screenshots/screenshot_6_5MMPK4p.png)
- [Auto Move Windows](https://extensions.gnome.org/extension/16/auto-move-windows/) - to move applications to specific workspaces when they are launched.
  - I use this to launch Spotify on my last workspace, for example.
- [Extend Panel Menu](https://extensions.gnome.org/extension/1201/extend-panel-menu/) - to seperate the Power/Network/Volume/User/Date/Notification menus into their own indicators in the status area, as opposed to the default of them all merged into one, big menu.
  - I enable `Autohide the Notification Indicator`
- [No Title Bar](https://extensions.gnome.org/extension/1267/no-title-bar/) - moves the titlebar to to top panel when the window is maximized or split left/right
  - ![](https://extensions.gnome.org/extension-data/screenshots/screenshot_1267.png)
- [Places Status Indicator](https://extensions.gnome.org/extension/8/places-status-indicator/) - for a quick Explorer launcher when in Mouse-mode
  - ![](https://extensions.gnome.org/extension-data/screenshots/screenshot_8_mVLeGic.png)
- [Removable Drive Menu](https://extensions.gnome.org/extension/7/removable-drive-menu/) - A status menu for accessing and unmounting removable devices
- [Sound Input & Output Device Chooser](https://extensions.gnome.org/extension/906/sound-output-device-chooser/) - enhances Volume Indicator with input and output pickers
- [TaskBar](https://extensions.gnome.org/extension/584/taskbar/) - display icons of running applications, current workspace number, and button for Application Overview
  - I disable `Tasks` and `Desktop Button`
- [Top Panel Workspace Scroll](https://extensions.gnome.org/extension/701/top-panel-workspace-scroll/) - change workspaces by scrolling over the top panel when in Mouse-mode
- [TopIcons Plus](https://extensions.gnome.org/extension/1031/topicons/) - moves legacy tray icons (bottom left of Gnome Shell) to the top panel

## MacOS-like
- Quick Look -> [Gnome Sushi](http://www.omgubuntu.co.uk/2016/09/gnome-sushi-mac-quick-look-nautilus)
  - press `Spacebar` when selecting a file to see a preview of it
- Spotlight -> Comes with Gnome Shell
  - Just press `Super` and start typing
- Spaces -> called Workspaces now
- Hot Corners -> [CustomCorner](https://extensions.gnome.org/extension/1037/customcorner/)
- MenuBar's App Menu -> [Gnome Global AppMenu](https://github.com/lestcape/Gnome-Global-AppMenu)
  - I am not currently using this, but it [looks](http://www.omgubuntu.co.uk/2017/04/global-menu-for-gnome-extension-development) useful
- Searchable commands (`super /`) -> [Plotinus](https://github.com/p-e-w/plotinus)
  - ![](https://cloud.githubusercontent.com/assets/2702526/20246717/454a1a9a-a9e3-11e6-8b19-4db092348793.gif)

## Window Management
- Use Workspaces
  - `Tweak Tool` ->  `Workspaces` -> `Workspace Creation` set to `Static`
  - `Super 1-4` to switch to them (set in `Settings` -> `Keyboard`)
- [gTile](https://extensions.gnome.org/extension/28/gtile/) to position windows

  I use a 6 x 2 grid where:

  `Super Ctrl A` - Left

  `D` - right

  `Q` - top left

  `E` - top right

  `Z` - bottom left

  `C` - bottom right

  `F` - full screen

  `S` - middle 4 columns

  `1` - left 1/3

  `2` - middle 1/3

  `3` - right 1/3

  `Super Ctrl Shift 1` - left 2/3

  `Super Ctrl Shift 2` - middle 2/3

  `Super Ctrl Shift 3` - right 2/3

- If you'd like an auto-tiling window manager, consider [ShellTile](https://extensions.gnome.org/extension/657/shelltile/) or [shellshape](https://extensions.gnome.org/extension/294/shellshape/)
- CustomCorner
  - bottom left corner locks screen with this command: `dbus-send --type=method_call --dest=org.gnome.ScreenSaver \ /org/gnome/ScreenSaver org.gnome.ScreenSaver.Lock`

## Keyboard Setup
#### Remapping
`Gnome Tweaks` -> `Typing`
- `Miscellaneous compatibility options`
  - enable `Both shift keys together activate Caps Lock, on Shift key deactivates`
- `Ctrl key position`
  - enable `Left Alt as Ctrl, Left Ctrl as Win, Left Win as Alt`
- `Caps Lock key behavior`
  - enable `Make Caps Lock an additional Super`
- `Alt-Win key behavior`
  - enable `Alt is swapped with Win`

#### Custom Hotkeys
See [this](https://askubuntu.com/questions/254424/how-can-i-change-what-keys-on-my-keyboard-do-how-can-i-create-custom-keyboard/304834#304834) SO answer for a great writeup of [AutoKey](https://apps.ubuntu.com/cat/applications/autokey-gtk/)

> Unlike xmodmap, AutoKey doesn't rebind the actual keys on your keyboard; it runs in the background and intercepts your defined keyboard shortcuts, then sends simulated keypresses to your applications.

Using its `Phrases`, I have mapped things like `Super c` to `Ctrl c` for copy, and `Super h/j/k/l` to arrow keys.

#### Custom Keyboard
Only works w/ xmodmap in a DE using X11.

https://github.com/alols/xcape allows using modifier key as another key when pressed and released on its own.

https://github.com/jackrosenthal/threelayout