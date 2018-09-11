```
._____           _     
|_   _|__   ___ | |___
  | |/ _ \ / _ \| / __|
  | | (_) | (_) | \__ \
  |_|\___/ \___/|_|___/
```

# VS Code
## Tips
- see [Microsoft/vscode-tips-and-tricks: Collection of helpful tips and tricks for VS Code.](https://github.com/Microsoft/vscode-tips-and-tricks)
- [awesome-vscode: A curated list of delightful VS Code packages and resources.](https://github.com/viatsko/awesome-vscode)
- [Tasks in Visual Studio Code](https://code.visualstudio.com/docs/editor/tasks)
- Use Breadcrumbs!
- [Set up CLI `code` command](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)
- [Disable tabs](https://stackoverflow.com/questions/38147154/how-to-disable-tabs-in-vscode)
  - `Close all editors in group` to remove split/pane. Otherwise, `cmd-w` will close a file, but the split will still
    remain if other files have been open in that split.


## Hotkeys/commands
- `cmd-shift-p` (Command Palette)
  - `"sort lines"`
- `cmd-shift-o` nav to symbol
- `cmd-shift-.` focus breadcrumbs
  - `cmd-left/right` move up/down in breadcrumbs
- `shift-option-o` for outline of file for quick nav
- `ctrl-q` open quick switch to section of app
- `ctrl-l` codeFileNav (vinegar.vim)
- `cmd-shift-e` toggle switch to file explorer
- `cmd-\` split editor
- `cmd-shift-o` find by symbol
- `cmd-shift-v` toggle markdown preview
- `cmd-k z` zen mode

## Settings
#### Disable minimap
```
"editor.minimap.enabled": false,
```


## Settings Plugins
#### [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)
- This is the first thing you should install and set up - great for backing up and syncing the same config across machines.
- Follow steps in Sync readme to set up a Github Key.
- After install, be sure to `Sync: Advanced Options > Toggle Auto-Upload` and `Toggle Auto-Download` to force staying in sync.

#### [TSLint](https://marketplace.visualstudio.com/items?itemName=eg2.tslint) for linting `.ts` [rules](https://palantir.github.io/tslint/rules/)
- [buzinas/tslint-eslint-rules: Improve your TSLint with the missing ESLint rules](https://github.com/buzinas/tslint-eslint-rules)
- [palantir/tslint-react: Lint rules related to React & JSX for TSLint.](https://github.com/palantir/tslint-react)
- [Microsoft/tslint-microsoft-contrib: A set of TSLint rules used on some Microsoft projects.](https://github.com/Microsoft/tslint-microsoft-contrib)
- [vrsource/vrsource-tslint-rules: A extra set of tslint rules](https://github.com/vrsource/vrsource-tslint-rules)

Recommendation: start with
```js
"extends": ["tslint:latest", "tslint-react"]
```
and trim back rules as you see fit. For reference, `tslint:latest` is a combination of [latest](https://github.com/palantir/tslint/blob/master/src/configs/latest.ts) and [recommended](https://github.com/palantir/tslint/blob/master/src/configs/recommended.ts) rules.

#### [Trailing Spaces](https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces)
![](https://shardulm94.gallerycdn.vsassets.io/extensions/shardulm94/trailing-spaces/0.2.11/1474455467376/Microsoft.VisualStudio.Services.Icons.Default)

#### [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
Everything you could need for git analysis (history, blame, diff). Not for commit and branch management - that is baked in by default.
![](https://raw.githubusercontent.com/eamodio/vscode-git-codelens/master/images/preview-gitlens.gif)

## Navigation
#### [File Navigator](https://marketplace.visualstudio.com/items?itemName=jakelucas.code-file-nav)
Closest thing to vinegar.vim

#### [Duplicate file](https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-duplicate)
Add missing `Duplicate File` entry to File Explorer right-click menu.

OR just copy/paste, then rename the file without this extension

#### [Markdown Navigate](https://marketplace.visualstudio.com/items?itemName=jrieken.md-navigate)
![](https://raw.githubusercontent.com/jrieken/md-navigate/master/demo.gif)

#### [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek)
![](https://github.com/pranaygp/vscode-css-peek/raw/master/images/working.gif)


## Editing Plugins
#### [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
Automatically closes tags while writing the first one, and can close tags after the fact with `cmd-alt-.`

#### [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
Currently has a [bug](https://github.com/formulahendry/vscode-auto-rename-tag/issues/19) with multi-line tags though

![](https://raw.githubusercontent.com/formulahendry/vscode-auto-rename-tag/master/images/usage.gif)

#### [htmltagwrap](https://marketplace.visualstudio.com/items?itemName=bradgashler.htmltagwrap)
Select a chunk of code and press `alt-w` to wrap code in a tag

#### [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
Visual Studio Code plugin that autocompletes filenames.

![](http://i.giphy.com/iaHeUiDeTUZuo.gif)

## Colors
#### [Dracula Official](https://marketplace.visualstudio.com/items?itemName=dracula-theme.theme-dracula)
Best colorscheme among all editors :)

![](https://draculatheme.com/assets/img/screenshots/vscode.png)

#### [Babel JavaScript](https://marketplace.visualstudio.com/items?itemName=mgmcdermott.vscode-language-babel)
Ported syntax highlighting from Atom

#### [Output Colorizer](https://marketplace.visualstudio.com/items?itemName=IBM.output-colorizer&cm_mc_uid=27674934593514849743568&cm_mc_sid_50200000=1484974356)
Syntax highlighting for log files

![](https://raw.githubusercontent.com/IBM-Bluemix/vscode-log-output-colorizer/master/github-assets/screenshot-4.jpg)

#### [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
Highlight `TODO`, `FIXME` or any annotations within your code.

![](https://github.com/wayou/vscode-todo-highlight/raw/master/assets/material-night.png)


## Tools
#### [vscode-chrome-debug](https://github.com/Microsoft/vscode-chrome-debug)
Debug your JavaScript code running in Google Chrome from VS Code.

#### [Color Info](https://marketplace.visualstudio.com/items?itemName=bierner.color-info)
Provides additional information about css colors.

![](https://github.com/mattbierner/vscode-color-info/raw/master/media/starter-example.png)

## Vim
#### Why VSCode instead of Vim?
- Main reason: **intellisense**.
- Also, freedom to customize. I don't want to write an auto-tag close feature for vim. I can easily with ts and vscode though. And because it is ts, I will have intellisense to help me. Unlike atom's CoffeeScript or vim's vimscript.
- vscode interates quickly, and in the open
- vscode works _well_ on Windows. I'm considering a switch, and the smoother the transition, the better.
- vscode format-on-save is great
- vscode is like iphone hardware with ios. The tight integration makes for a wonderful, first-class typescript experience.

Things I would miss from vim: **the details**. Got my syntax highlighting exactly the way I wanted. Marker folding was great for hiding import statements. Buffers, splits, and tabs for code viewing and organizing is huge to me, as mentioned in **TODO** vim doc.

Vim is like Linux. Loved customizing it to be (almost) exactly what I wanted, but takes so much time to get it and keep it there. vsCode is like MacOS - sane defaults with fewer customizations and little - no maintenance cost.

#### [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim) and its [roadmap](https://github.com/VSCodeVim/Vim/blob/master/ROADMAP.md) of what is available today

You'll want to enable holding down `j` and `k` with
```bash
defaults write com.microsoft.VSCode ApplePressAndHoldEnabled -bool false
defaults write com.microsoft.VSCodeInsiders ApplePressAndHoldEnabled -bool false
```

consider using these settings:
```json5
"editor.lineNumbers": "relative"
"vim.leader": " ", // map leader to <space>
"vim.hlsearch": true,
"vim.useSystemClipboard": true,
"vim.easymotion": true, // press `<space><space> s` to jump to a character

// fixes c-d, c-u for visual select. see https://github.com/VSCodeVim/Vim/issues/907#issuecomment-264738452
"vim.otherModesKeyBindingsNonRecursive": [
    {
        "before": ["<C-u>"],
        "after": ["2", "5", "k"]
    },
    {
        "before": ["<C-d>"],
        "after": ["2", "5", "j"]
    },
    {
        "before": ["<C-f>"],
        "after": ["5", "0", "j"]
    },
    {
        "before": ["<C-b>"],
        "after": ["5", "0", "k"]
    }
],
```

#### Hotkeys/commands
- `gh` - show hover tooltip
- `gb` - add an additional cursor at the next place that matches *


## Emacs
#### [Emacs](https://marketplace.visualstudio.com/items?itemName=hiro-sun.vscode-emacs)
#### [keyboard-scroll](https://marketplace.visualstudio.com/items?itemName=selbh.keyboard-scroll) to enable `ctrl-l` functionality
#### [jumpy](https://marketplace.visualstudio.com/items?itemName=wmaurer.vscode-jumpy) (doesn't work with Emacs-plugin [yet](https://github.com/Microsoft/vscode/issues/13441)) for an Ace-Jump alternative
