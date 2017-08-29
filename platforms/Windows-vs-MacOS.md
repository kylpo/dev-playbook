# Default user experience
Realistically, despite these platforms being so customizable, most users will just use what comes out of the box. They'll use Edge, they'll use Safari. So, what will they experience?

## Mac has, Windows doesn't
- Widgets
- keyboard shortcut standards for preferences `cmd ,`
- standardized app toolbar (that lives in Menubar)
    - all options searchable with `cmd ?`
- Spotlight to easily preview content before officially opening
- App store with desktop-quality apps
    - though Windows just opened up their store to desktop apps
- Bash built in

## Windows has, Mac doesn't
- Gaming
    - And a focus of the OS with the recently added Game Bar
- Window manager via hotkeys
    - `Win + left/right` is readily available, with the helper selection to fill the other half of the screen. Nice!
- More themeing options than dark/light

# A primary platform difference: Bars
Mac's Menubar and Dock (bar) have some subtle, but important differences from Window's Taskbar.

|  macOS            |  Windows |
|---------------------|----------------------|
|![](https://developer.apple.com/macos/images/macos-hero-large.png) | ![https://www.tekrevue.com/tip/remove-clock-windows-10-taskbar/](https://cdn1.tekrevue.com/wp-content/uploads/2015/08/windows-10-taskbar-clock.jpg) |

Quickly, here are some terms:
- App Launcher: on press, will launch or focus an app. Can also close apps via this control.
- App Menu: contains menu options like `File`, `Edit`, `View`, etc for an app.
- System Tray (SysTray for short, also called Status Menus): is an extension point for icons and text to display information, open windows/dropdowns, and quick actions.

## MacOS opts for two bars
The bottom Dock is the App Launcher, consisting only of icons.

![https://support.apple.com/kb/PH25709?viewlocale=en_US&locale=en_US](https://support.apple.com/library/APPLE/APPLECARE_ALLGEOS/Product_Help/en_US/PUBLIC_USERS/PL124/S0041_Dock.png)

The top Menubar consists of the currently focussed app's menu (App Menu) on the left, and persistent status menus (SysTray) on the right.

![https://support.apple.com/kb/PH25077?locale=en_US](https://support.apple.com/library/APPLE/APPLECARE_ALLGEOS/Product_Help/en_US/PUBLIC_USERS/PL124/S0010_Menubar.png)

Two things to note here versus Windows.
1. Individual apps do not have App Menus in their Window. They will always appear in the MenuBar. Some argue this is good for mouse users (consistent location), some argue it is bad (window on right side of screen needs has menus on left side)
2. Icons AND TEXT allowed in the SysTray, only icons are allowed, which is a huge bummer for developers building timers, calendar notifications, etc.
    - ![](http://is3.mzstatic.com/image/thumb/Purple7/v4/f3/74/c0/f374c029-5ac9-0abe-7e57-71e9aa1f811f/source/800x500bb.jpg)


## Windows opts for one bar
The app launcher lives on the left side, and has a bit more power than MacOS's Dock.
1. It can be expanded to include text (not just icons):
    - ![https://www.howtogeek.com/225568/how-to-configure-and-customize-the-taskbar-in-windows-10/](https://www.howtogeek.com/wp-content/uploads/2016/11/xwtt_30-650x99.png.pagespeed.gp+jp+jw+pj+ws+js+rj+rp+rw+ri+cp+md.ic.y1d1qhtSiw.png)
2. Hovering over an icon shows a preview and potentially some actions
    - ![https://msdn.microsoft.com/en-us/library/windows/desktop/dd378460%28v=vs.85%29.aspx?f=255&MSPPError=-2147217396#thumbbars](https://i-msdn.sec.s-msft.com/dynimg/IC420540.png)
3. A progress indicator can be used in creative ways, like [Taskbar Meters](http://taskbarmeters.codeplex.com/) has done
    - ![https://www.techjunkie.com/add-system-resource-desktop/](https://i2.wp.com/www.techjunkie.com/wp-content/uploads/2016/05/system-resource7.jpg?w=329&ssl=1)


its persistent SysTray lives on the right.





## Bars
Mac will have Dock and Menubar visible

Windows will just have the bottom Taskbar visible