_WIP_

## Hotkeys
Be sure to start with a `Keymap` that you like. I prefer `Emacs`.

[No Tabs in IntelliJ IDEA – Hadi Hariri](http://hadihariri.com/2014/06/24/no-tabs-in-intellij-idea/)
- Hide tabs
- use ctrl-tab to switch buffers
- Recent Positions: `cmd [` to go back, `cmd ]` to go forward
- Recent Files
- use the Navigation Bar

[Kye Hohenberger on Twitter: "This is really cool. @WebStormIDE import autocomplete works so well I hardly noticed it the first time. https://t.co/Tne3w1IywX"](https://twitter.com/tkh44/status/878368684850520064)

Customize syntax highlighting to support template literals (I think) - [Webstorm, IntelliJ 등의 JetBrains IDE에서 styled-components 사용하기](https://medium.com/@iamssen/webstorm-intellij-%EB%93%B1%EC%9D%98-jetbrains-ide%EC%97%90%EC%84%9C-styled-components-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0-b0bc79418e1f)

## Settings
### Format on save
From [7 reasons this Android Code Style improves your productivity](https://android.jlelse.eu/7-reasons-this-android-code-style-improves-your-productivity-65d196fa55f)

- Select Edit > Macros > Start Macro Recording
- Select Code > Optimize Imports
- Select Code > Reformat Code
- Select Code > Rearrange Code
- Select File > Save All
- Select Edit > Macros > Stop Macro Recording and give it a name (mine is OptimizeImportsReformatRearrangeSave)
- Go to Preferences > Keymap
- Find the Macro section
- Add ⌘ + S shortcut for the new macro

## Plugins
[Styled Components :: JetBrains Plugin Repository](https://plugins.jetbrains.com/plugin/9997-styled-components)

![](https://pbs.twimg.com/media/DIpJ6nSWAAEXsKh.jpg)

[JetBrains WebStorm on Twitter: "If you’re using styled\-components 💅, you should definitely try this new plugin: https://t\.co/bWFPSlNKEl https://t\.co/YbF2evFA0x https://t\.co/81XVyKbRzZ"](https://twitter.com/WebStormIDE/status/903615955032518656)

## Developing Plugins
- Dig in to source code of [styled\-components/webstorm\-styled\-components](https://github.com/styled-components/webstorm-styled-components) for a plugin built with Kotlin
- [JetBrains/gradle\-intellij\-plugin: Plugin for building plugins for IntelliJ IDEs](https://github.com/JetBrains/gradle-intellij-plugin)
- [Creating Your First Plugin / IntelliJ Platform SDK DevGuide](https://www.jetbrains.org/intellij/sdk/docs/basics/getting_started.html)
- [Reference \- Kotlin Programming Language](https://kotlinlang.org/docs/reference/)