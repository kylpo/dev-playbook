# Windows
From the onset, you have a difficult decision to make. Do you build your app with Universal Windows Platform (UWP), with its sandboxed, siloed, limited feature set, but modern, active SDK? Or do you build with the legacy Win32 platform, with fully feature-capable, aging documentation, and only recently app-store capable?

Want to see the differences of UWP to Win32? Try out Evernote from the store vs website. Try out Todoist from the store vs website. Onenote, Outlook. Or just the good ole Notes Win32 app vs a popular one on the app store like [Dark Note](https://www.microsoft.com/en-us/store/p/dark-note/9wzdncrdkm2g?SilentAuth=1&wa=wsignin1.0&rtc=1).

## BIG differences
- Global hotkeys
- UWP siloed to its own window. The Notes app cracks me up: no floating/pinnable windows. You'd have to split the app to see a note when multitasking. Thank goodness it is visible as a Metro Tile though (which immediately goes away when it loses focus)! :P
    - ![](https://store-images.s-microsoft.com/image/apps.59052.9007199266524105.10886cce-b950-4609-9669-fbe3bcf28707.c30aee79-c91f-484f-bc32-bf044b580043?w=1399&h=787&q=60)
    - ![](https://store-images.s-microsoft.com/image/apps.11744.9007199266524105.427455f1-c678-4772-9db7-f763c683a818.80353b55-c0cb-4d57-9c2d-356e2719f6f1?w=1399&h=787&q=k60)

Honestly, both roads kind of suck, but UWP's limitations are essentially a non-starter, which is why the app store has been so baren for the past 5 years, so Win32 with Desktop Bridge ([link1](https://docs.microsoft.com/en-us/windows/uwp/porting/desktop-to-uwp-root), [link2](https://developer.microsoft.com/en-us/windows/bridges/desktop)) to host the app on the Store is really the only option. This recent Desktop Bridge capability (once called [Project Centennial](https://www.windowscentral.com/windows-10-anniversary-update-project-centennial-apps-store)) is why we are now, finally seeing "real" apps in the app store, like [Spotify](https://www.windowscentral.com/spotify-coming-windows-10-store-pc), [Office](http://www.zdnet.com/article/microsoft-broadens-office-365-through-the-windows-store-test-program/#ampshare=http://www.zdnet.com/article/microsoft-broadens-office-365-through-the-windows-store-test-program/), others?.

Why use Desktop Bridge?

Well, you don't really have to, but Microsoft continues to push down the path of a Store-only OS. The push started with Windows RT and is now being rebranded as Windows 10S (for "students").


## Where should it live?

#### Taskbar
Capabilities:

Considerations:

<!-- #### Dock
- Not just for launching. Can also show information.
- Just update the icon with information. See the built-in Activity Monitor, for example:
- ![](https://github.com/kylpo/dev-playbook/blob/master/assets/activity-monitor-icon.png?raw=true)
- Can also launch popups, like those shown in menubar. -->

#### Window
Considerations:

#### Floating window
- Above all others
- Often no titlebar
- Examples
    - [Window On Top, Always On Top, Windows On Top, How to keep any window on top, Download, Windows Software](http://www.skybn.com/window-always-on-top/)
    - [Make a window stay Always On Top in Windows 10/8/7](http://www.thewindowsclub.com/make-a-window-stay-always-on-top-windows) 
    - [The 3 Best Ways to Make a Window Always\-on\-Top on Windows](https://www.howtogeek.com/196958/the-3-best-ways-to-make-a-window-always-on-top-on-windows/)
- Means you can essentially take over regions of the screen
    - ...

Considerations:

- adjustable opacity?
- adjustable style (to match user's background)?
- able to toggle "always on top"?
- resizable?
- global hotkeys?

#### Pinned to desktop (Desktop Widget)
- Pinned
- No titlebar
- Power users would have "easy" access to these via the `win d` hotkey to `Show Desktop`

Considerations:

- adjustable opacity?
- adjustable style (to match user's background)?
- able to toggle "always on top"?
- resizable?
- global hotkeys?


#### Misc
Note that you can use webviews to display web content in these locations, too.

## Extension Points
### Open to all types
#### Notifications

#### Context Menu
- Not necessarily where it lives, more of how it is invoked. This is an `extension`.

#### Actions

#### Share

### If your app is document-based