# Dev setup
- [How to set up the perfect modern dev environment on Windows](http://char.gd/microsoft/setting-up-perfect-windows-dev/)
- [My Bash on Windows Dev Environment - daverupert.com](http://daverupert.com/2017/03/my-bash-on-windows-developer-environment/)
- [How to Show Hidden Files in Windows 10 - Winaero](http://winaero.com/blog/show-hidden-files-windows-10/)
- [Setting up a Shiny Development Environment within Linux on Windows 10 - Scott Hanselman](https://www.hanselman.com/blog/SettingUpAShinyDevelopmentEnvironmentWithinLinuxOnWindows10.aspx)
- Terminal
  - [Everything You Can Do With Windows 10’s New Bash Shell](https://www.howtogeek.com/265900/everything-you-can-do-with-windows-10s-new-bash-shell/)
  - [Terminus](https://eugeny.github.io/terminus/)
    - ![](https://github.com/Eugeny/terminus/raw/master/docs/linux.png)
  - or Hyper
    - [johnlindquist ✌ on Twitter: "@reybango @rauchg @freebly @_developit @msdev @Microsoft @surface @richturn_ms In your `.hyper.js` (which is the hyper settings file) change the shell to "shell: 'c:\\windows\\System32\\bash.exe'," https://t.co/YSJOvDCFPP"](https://twitter.com/johnlindquist/status/859864517672488960)
- [Zach Bruggeman on Twitter: "i've been using the latest WSL for a bit, could see this replacing my mac for dev work. @zeithq's hyper is a great terminal for windows https://t.co/PYFKdoEWFY"](https://twitter.com/zachbruggeman/status/853340648983773184)
  - ![](https://pbs.twimg.com/media/C9eql3jUwAA_RaV.jpg)
- [Neovim on Twitter: "#neovim 0.2 is out: https://t.co/PAWUEgPT8M * Official Windows support * Pre-build macOS package * :terminal improvements * ... and more!"](https://twitter.com/Neovim/status/859317754687631361)
- [Setting up a Shiny Development Environment within Linux on Windows 10 - Scott Hanselman](https://www.hanselman.com/blog/SettingUpAShinyDevelopmentEnvironmentWithinLinuxOnWindows10.aspx)
- [Max Stoiber on Twitter: "@yosefdurr If anybody has tips for must-have Windows apps (Mac/Rocket-like emoji keyboard?!) please let me know! #maxgoeswindows"](https://twitter.com/mxstbr/status/878380743595929600)

# Familiar to MacOS
- [Essential apps for switching from Mac to Windows - Charged](https://char.gd/blog/2017/essential-apps-for-switching-from-mac-to-windows)
- Spotlight
  - [hainproject/hain: An 'alt+space' launcher for Windows, built with Electron](https://github.com/hainproject/hain)
    - ![](http://hainproject.github.io/hain/images/demo.gif)
  - [Wox-launcher/Wox: Launcher for Windows, an alternative to Alfred and Launchy.](https://github.com/Wox-launcher/Wox)
    - ![](https://camo.githubusercontent.com/9db33546d3a905a9ad915e0948d3ba3f47f57b64/687474703a2f2f692e696d6775722e636f6d2f4474784e424a692e676966)
  - [Keypirinha](http://keypirinha.com/)
- [Add An OS X Like File Preview Feature To Windows 10](http://www.addictivetips.com/windows-tips/add-an-os-x-like-file-preview-feature-to-windows-10/?utm_source=feedburner&utm_medium=twitter&utm_campaign=Feed%3A+Addictivetips+%28AddictiveTips%29)
- [Jason Miller 🦊⚛ on Twitter: "People switching to Windows 10 from MacOS: Install this and bind it to ctrl + space. You're welcome. https://t.co/rWAHHsflAF"](https://twitter.com/_developit/status/859791623638716417)
- OS-level emacs keybinds (like MacOS)
  - [usi3/emacs.ahk: An autohotkey script that allows you to use emacs-like key bindings on Windows environment](https://github.com/usi3/emacs.ahk)
  - or the easier to configure [fujieda/xkeymacs](https://github.com/fujieda/xkeymacs) (be sure to use the snapshot version). Problem with this one is that it doesn't affect some system level inputs, like the `win` key search or `Explorer` address bar.
- Spaces
  - Virtual Desktops exist in Windows 10 now!
  - But, for whatever reason, there isn't a keybind to jump directly to a Space (`ctrl 1` by default to jump to Space 1, `ctrl 5` to jump to Space 5)
  - Use [win\-10\-virtual\-desktop\-enhancer](https://github.com/sdias/win-10-virtual-desktop-enhancer/blob/master/docs/settings.md#keyboard-shortcuts) to get the jump hotkeys. Also a nice little display to tell you what Space you jumped to.
- Hot Corners
  - [WinXCorners — Hot Corners for Windows 10](http://apps.codigobit.info/2015/10/winxcorners-hot-corners-for-windows-10.html)
  - I like my bottom-left corner to lock screens, so I use the custom action to `rundll32.exe user32.dll,LockWorkStation` and set to bottom-left.
    - Found that command from [Command\-line \(cmd\) command to lock a windows machine \- Super User](https://superuser.com/questions/21179/command-line-cmd-command-to-lock-a-windows-machine)
  - ![](http://lh3.googleusercontent.com/-vxIVdOymPXY/Vh-ze0Bn4bI/AAAAAAAALQY/zZ9TGvPVQpE/WinXCorners%25255B5%25255D.jpg?imgmax=800)
  - [How to Get Hot Corners in Windows 10 \- Make Tech Easier](https://www.maketecheasier.com/get-hot-corners-windows-10/) for a nice write-up

# Window Management
- use [WinDivvy](http://mizage.com/windivvy/) to move/position windows with your keyboard. Closest Windows app I could find to [Moom](https://manytricks.com/moom/).
  - ![](http://mizage.com/windivvy/screenshots/shortcuts.png)

# Utils
- Desktop Widgets
  - [Win10 Widgets \- Widgets for Windows 10](http://win10widgets.com/)
  - ![](http://win10widgets.com/images/screenshot.png)
  - [How to Create an Attractive, Customized Desktop HUD with Rainmeter](http://lifehacker.com/5828789/how-to-create-an-attractive-customized-desktop-hud-with-rainmeter)
- Remap keys with [sharpkeys: SharpKeys is a utility that manages a Registry key that allows Windows to remap one key to any other key\.](https://github.com/randyrants/sharpkeys)
  - I use it to replace:
    - `caps_lock` -> `win`
    - `left_alt` -> `left_ctrl`
    - `left_win` -> `right_alt`
- Focus of active window
  - 

# Settings
- [How To Reverse Scroll Direction In Windows 10](http://www.addictivetips.com/windows-tips/reverse-scroll-direction-in-windows-10/)
- [How to Disable Animations in Windows (and Make It Feel Faster)](http://lifehacker.com/how-to-disable-animations-in-windows-and-make-it-feel-1728734414)
- [Audit and Optimize your Windows 10 Search Indexing Options - Scott Hanselman](https://www.hanselman.com/blog/AuditAndOptimizeYourWindows10SearchIndexingOptions.aspx)
- [How to Disable All of Windows 10’s Built-in Advertising](https://www.howtogeek.com/269331/how-to-disable-all-of-windows-10s-built-in-advertising/)
- "If you haven't already, I highly recommend you configure Hey Cortana to respond only to your voice" - [Jen Gentleman 🌺 on Twitter](https://twitter.com/JenMsft/status/890410962200678400)
  - ![](https://pbs.twimg.com/media/DFtfc_0VoAEUEL1.png)

# Tools
- [Microsoft Snip brings Windows screenshots to life with voice and ink](https://www.theverge.com/2015/8/27/9214079/microsoft-snip-windows-screenshot-tool)
