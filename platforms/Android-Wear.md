Note: Below's notes are just summarizing [Introduction \- Android Wear \- Android Wear design guidelines](https://www.google.com/design/spec-wear/android-wear/introduction.html). Be sure to flip through those pages.

# Architecture
Android Wear 2.0 is all about 1-dimensional, vertical columns. Horizontal can still play a role, but it is secondary, and lives inline to the vertical column (think carousels).

This <img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B5QhgrCEXHzxZExrQUxveTFTa2s/optimize_for_vertical_layout_1.png" width="300"/>, not <img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B5QhgrCEXHzxNW1aLUFGanJWNjA/optimize_for_vertical_layout_2.png" width="300"/>

## 3 Primary Views/Columns
### Main
Your default column houses your `Watch Face` at the top, and any `collapsed notifications` below it.

#### Watch Face
![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B5QhgrCEXHzxQTFWT1RPRFAydVk/02_watch_faces.png)

[Interactive watch faces \- Patterns \- Android Wear design guidelines](https://www.google.com/design/spec-wear/patterns/interactive-watch-faces.html#) for more

#### Collapsed Notifications
![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDTTNibUJ1Nm5pREE/notifications_anatomy_stream_card_callouts.png)

1. A large icon (optional)
2. An app icon
3. A content title
4. Content text
5. Primary action

from [Notifications \- Patterns \- Android Wear design guidelines](https://www.google.com/design/spec-wear/patterns/notifications.html#notifications-templates)

### Notification Detail (expanded notification)
Upon clicking on a collapsed notification, you are taken to a new view/column: the expanded notification. To get back to the main column, swipe right. Imagine expanded notifications living in a column to the right of the main column.

![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDY3VBNXdBZENkVHc/notifications_anatomy_appoid_callouts.png)

1. A content title
2. An app name
3. An app icon
4. Content text
5. A big picture (optional)
6. Inline action: If you have a primary action in a collapsed notification, you should add the same action here.
7. Smart replies: If the notification is MessagingStyle, the system can show smart suggestions
8. Action drawer: Add any remaining notification actions in this area. The user can swipe up or tap the overflow icon to open the drawer.

from [Notifications \- Patterns \- Android Wear design guidelines](https://www.google.com/design/spec-wear/patterns/notifications.html#notifications-templates)

### App
An app is navigated to by a pre-programmed hardware key, by voice, or by the app launcher (shown below).

![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B5QhgrCEXHzxRXBTZ2JhR2ZrZDA/03_apps.png)

When it is active, its view takes over (much like an expanded notification), but has some additional components to leverage. Best to think of it as a `Viewport` layer at the lowest position, and two layers floating over it at the top position (`Navigation Drawer`) and bottom position (`Action Drawer`). Note: both drawers use a `peek` animation to inform the user of their existence.

![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B5QhgrCEXHzxRGhucC1XZ0w3eGs/orthographic_view_of_app.png)

#### The `Viewport` contains:
- content (text, images, etc). See [Content containers \- System overview \- Android Wear design guidelines](https://www.google.com/design/spec-wear/system-overview/content-containers.html) for more.

<img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDMkIzMFRNZ2dqcmc/vert_page.png" width="400"/> <img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDMFVIckI1dXJqbVE/pannable_view.png" width="400"/>

- a optional, big [Primary action button](https://www.google.com/design/spec-wear/components/primary-action-buttons.html#) (hierarchically outside of content)

<img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDM2IwX0hYcnVkeUE/primary_button_label.png" width="200;" />

- and optional [Inline action buttons \- Components \- Android Wear design guidelines](https://www.google.com/design/spec-wear/components/inline-action-buttons.html#) shown after content (hierarchically inside of content)

<img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDdXJmVURqczJxNEk/inline_action_button.png" width="200" />

#### [Navigation Drawer](https://www.google.com/design/spec-wear/components/navigation-drawer.html#navigation-drawer-behavior)
If used, will have 2+ horizontal tabs that when actived change the `Viewport`. Much like tabs in your browser.

![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDMUl1WVVfcHlhS28/usage.png)

Can also be collapsed into a single page of multiple buttons.

<img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B7l-XnaAL2nDZjZrTWhhbTZzZUU/navigation_drawer_singlepage.png" width="200;"/>


#### [Action Drawer](https://www.google.com/design/spec-wear/components/action-drawer.html#)
A vertical sheet that, when expanded, includes additional actions.

<!-- <img src="" width="300"/> -->
<img src="https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B5QhgrCEXHzxQm5QRFZyTzhnQU0/action_drawer_open.png" width="200"/>

# Display Modes
![](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_images/Android-Wear-watches.gif)

from [Android Wear: wear what you want, get what you need](https://www.blog.google/products/android-wear/android-wear-wear-what-you-want-get/)

## Active Mode
Shows all, bright colors and animations. You just pressed something to wake up the watch.

![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B2SJIKn8-BKoMzMxWlRWd0JvU3c/pfadm-01.png)

## Always-on Mode (also called Ambient Mode)
Dims screen to grayscale to conserve battery. The more black space on the screen, the more battery is saved.

![](https://storage.googleapis.com/material-design/publish/wear_v_3/assets/0B2SJIKn8-BKoNF9aRzdSci1mSTg/pfadm-02.png)

Note: Apps can take advantage of this, too! No longer just the Face.
- By default your app in ambient mode only updates the screen every minute. This can be changed for time-sensative matters like timers and running apps.
- Read [Keeping Your App Visible \| Android Developers](https://developer.android.com/training/wearables/apps/always-on.html) for more.
- Watch [How to: Use Always\-on Apps with Android Wear \- YouTube](https://www.youtube.com/watch?v=_-xYB9EBTaA) for examples.

![](https://1.bp.blogspot.com/-Jz1tjR2Ouyc/VYyZ9thRtmI/AAAAAAAAAhE/wajr8jHut4Q/s320/Screen%2BShot%2B2015-06-25%2Bat%2B5.16.24%2BPM.png)

from [Official Android Blog: Android Wear: Always\-on apps](https://android.googleblog.com/2015/06/android-wear-always-on-apps.html)

# App Capabilities
- Watch this [fake climbing app](https://youtu.be/Hw37dxW6q5g?t=27m12s) demonstrating many capabilities
- Apps can be built as `Standalone` and installed directly from watch, not needing a paired phone. This opens more doors for the iOS story.

# App Dev
- Watch [Android Wear 2\.0: Building Apps with Material Design \- Google I/O 2016 \- YouTube](https://www.youtube.com/watch?v=LtD7eJp2ILo)
- [Creating and Running a Wearable App \| Android Developers](https://developer.android.com/training/wearables/apps/creating.html)
- [Building Apps for Wearables \| Android Developers](https://developer.android.com/training/building-wearables.html)

# Notification Dev
- Watch [What’s new with Notifications in Android N and Android Wear 2\.0 \- Google I/O 2016 \- YouTube](https://www.youtube.com/watch?v=6eFQbC5r17w)
- [Adding Wearable Features to Notifications \| Android Developers](https://developer.android.com/training/wearables/notifications/index.html)

# Watch Face Dev
- "Android Wear watch faces are services that are packaged inside a wearable app. When users select one of the available watch faces, the wearable device shows the watch face and invokes its service callback methods." - [Building a Watch Face Service \| Android Developers](https://developer.android.com/training/wearables/watch-faces/service.html#CreateProject)
- [Interactive watch faces \- Patterns \- Android Wear design guidelines](https://www.google.com/design/spec-wear/patterns/interactive-watch-faces.html#interactive-watch-faces-interactive-watch-faces) says only gesture allowed is single-tap, no swipes.
  - Though this app has left/right scrolling to reveal more tappable content: [Bubble Cloud Wear Launcher Watchface \- Android Apps on Google Play](https://play.google.com/store/apps/details?id=dyna.logix.bookmarkbubbles&referrer=utm_source%3D42matters.com%26utm_medium%3DWidgetWeb)
  - I'm confused
- You'll likely want to plan for [Complications](https://www.google.com/design/spec-wear/patterns/complications.html#complications-guidelines)

# Performance
  - [From Actions to battery life, these updates will make Android Wear 2.0 even better](https://www.wareable.com/android-wear/android-wear-updates-actions-battery-life-456)
    - "Did you also know that an all-white display can use up to seven times more power than a black display in interactive mode?"
    - "It also wants developers to be smarter with design choices to reduce battery suck, including making use of ambient mode and using fewer animations"
    - "did you know that Bluetooth is way more battery intensive than LTE or Wi-FI? Well it is, and Google wants developers to use the latter when possible to transfer data to Wear devices. It also wants developers to reduce the amount of vibrations and location checks."

# Tips
- [Android Wear tips and tricks: The hidden smartwatch secrets](https://www.wareable.com/android-wear/android-wear-hidden-secrets-tips-and-tricks)
  - pin favorite apps by holding it down in the launcher for a second
