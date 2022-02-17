---
author: Everett Wilson
paging: Is it over yet? (%d of %d)
---

# nvim+tmux
Terminal hacking like it's 2022.

---

## Why bother?
- [The Lindy Effect](https://en.wikipedia.org/wiki/Lindy_effect) - It's been
around longer than nearly anything else, and will outlive nearly anything else.
Because of this...
    - Immediate access to a huge array of utilities from the past.
    - Skills gained are an investment in the future.
- Live out the [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy)
and find the right tools for the job.
    - The only limits to what you can construct are your imagination and time.
    - (But the vastness of the open source ecosystem make it moreso the former)
- Scratch your own itch.
    - We all have those nagging idiosyncracies embedded in our workflow.
    Wouldn't it be nice to have them simply... go away?
- Make programming fun again.
    - There's something to be said for the homeliness of a well-curated set of
    dotfiles.
- Handle heterogenous programming
    - More on this in a moment

---

## Why this combination?
- [tmux](https://github.com/tmux/tmux) is the go-to terminal multiplexer, a
standout tool for handling a terminal-heavy workflow. Effectively used as a:
    - Window manager (a la `i3`)
    - Session persistence mechanism (a la `screen`)
    - Virtual workspace manager
- [neovim](https://neovim.io/) is a modernized fork of the classic text editor
that pares down support for legacy systems in order to:
    - Offer best-in-class extensibility via asynchronous plugin system
    - Integrate native LSP support for modern development experience
    - Offer a complementary Lua scripting engine that is taking the world by
    storm, while remaining fully backward compatible with the best of Vim
    - Set more sane defaults. Turns out, some things are nice to just have enabled

---

## What does this look like in action?
- Quick demo/office tour

---

## Replicating a modern development environment
"With great power, comes loads of cool-ass possibilities." - Uncle Ben, probably
- The essential components to turning an editor into an IDE:
    - Smart completion, and code comprehension (LSP server) - [Conquer of Completion](https://github.com/neoclide/coc.nvim)
        - Gets you 80% of the way there
        - Go to definition, smart rename, go to references, etc
    - Integrated fuzzy finding - [fzf](https://github.com/junegunn/fzf.vim)
        - Pair with [ripgrep](https://github.com/BurntSushi/ripgrep) to achieve
        nirvana
    - Filetree explorer - [nvim-tree](https://github.com/kyazdani42/nvim-tree.lua)
        - Because file picking feels better with vim motions
        - Presents useful information on git status
    - Status bar - [vim-airline](https://github.com/vim-airline/vim-airline)
        - Git integration, filetype information, file location information, errors, etc

---

## Making it feel like home
Small ideas that can help to make the experience a bit more personable. This is
entirely extra credit, just ideas for how to make things feel a bit nicer.
- Colorscheme - [gruvbox](https://github.com/gruvbox-community/gruvbox)
- List characters - `set listchars+=space:·`
    - Want to know why that whitespace isn't behaving like it should? This
    option solves all woes
- Everything Time Pope has ever done
    - Seriously, `vim-commentary` and `vim-surround` should just be upstreamed
    into (n)vim itself

---

## Thanks for listening
And I hope it was at least a fun listen.
