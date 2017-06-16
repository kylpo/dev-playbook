_Work in Progress_

```
._____           _     
|_   _|__   ___ | |___
  | |/ _ \ / _ \| / __|
  | | (_) | (_) | \__ \
  |_|\___/ \___/|_|___/
```

# Vim

# Why I always come back to vim
I get it. Your editor has better autocomplete. Your editor has better plugin management. Your editor has better syntax highlighting and theming.

I get it.

But what it does not have is the powerful combination of Buffers, Splits, and Tabs. I don't want or need an upside-down "L" shaped editor. I don't want a massive file tree explorer on the left side that when I click a file opens somewhere in the editor. I want to open a split, exactly where I want to open the file, open my tree view within that split, and open it right in that split.

vscode gives you up to 3 vertical splits, OR 3 horizontal splits. Totally sufficient when I am coding on my laptop, but most of my coding time is in front of a big monitor, and I can comfortably view 8 splits in vim (4 vertical, with 2 horizontal each).

Atom is much better with splits

I want to fuzzy-open easily from my open buffers, not just the recent 10 files I've visited.

And, no, I don't have any loyalty to vim or feel like my Schwartz is bigger than other nerds for using it. If this buffer/split/fileexplorer combination became available to vscode, I'd be there in a heart beat! Of course, then I might find something else that I miss too much from vim, like FZF, full control via keyboard, etc...


https://www.reddit.com/r/vim/comments/6axcij/spacevim_tabs_managersupport_fold_tabs/

[bagrat/vim-workspace: IDE-like Vim tabline](https://github.com/bagrat/vim-workspace)

# Oni
- https://github.com/extr0py/oni#configuration
- https://github.com/extr0py/oni/blob/master/browser/src/Config.ts#L34
- https://github.com/extr0py/oni/blob/master/ROADMAP.md

# Vimdiff
- [c	jump to previous hunk
- ]c	jump to next hunk
- dp	shorthand for `:diffput`
- :only	close all windows apart from the current one
- :Gwrite[!]	write the current file to the index
- :diffput pushes the hunk from the active buffer into the conflicted working copy
- http://vimcasts.org/episodes/fugitive-vim-resolving-merge-conflicts-with-vimdiff/

# Hotkeys
http://stackoverflow.com/questions/6264012/vim-delete-html-tag-but-not-content
- dst - delete surrounding tag
- yitvatp=at

Multi-file search/replace: use Ferret

Wrap w/ tag:
- ySit <Style_ background... <enter>
- capital S for new line after. lower s for same line.
- cst<p> - replace tag w/ <p>
- leader-p - fix indeting for whole file
- visual: gC - block comment
- gf - go to file
- gn - select next search match <- very useful
- ctrl-o - jump back
- ctrl-i - jump forward
- ^ - moves to start of line
- == - fix line's indentation
- K - Ag current word
- \ - Ag

# autocomplete
- https://github.com/prabirshrestha/asyncomplete.vim
- https://twitter.com/PrabirShrestha/status/848672199279992837
- https://github.com/jordwalke/VimBox/issues/36#issuecomment-292446541

# tmux integration
- https://blog.bugsnag.com/tmux-and-vim/
