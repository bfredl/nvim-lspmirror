# Nvim LSP Support MIRROR
This is a mirror of the [Nvim LSP PR](https://github.com/neovim/neovim/pull/6856) by @tjdevries. It is meant to be able to test and use the client without building from this branch. The code is written by TJ DeVries and not me (except minor fixes for running out-of-tree).

## Instructions
- Use recent Neovim master (or 0.3.2 when it is released)
- Add `bfredl/nvim-lspmirror` as a plugin in your `init.vim` (if you install this plugin as a standard vim plugin, you need to add ``set rtp+=...path/to/nvim-lspmirror`` before calling the following commands)
- Configure servers in your `init.vim`:
```
    call lsp#server#add(['c', 'c++'], ['clangd'], {})
    call lsp#server#add(['rust'], ['rls'], {})
```

- See `:help lsp` or discussion in the [PR](https://github.com/neovim/neovim/pull/6856) for further setup and usage instructions.
- Optional: add extension plugins:
  - `bfredl/nvim-lspext` for [inline diagnostics](https://user-images.githubusercontent.com/1363104/39083780-a8aeb2ac-456a-11e8-8901-15a24be634d1.png).
  - `shougo/deoplete-lsp` LSP Completion source for deoplete.

## Please report issues and suggestions to the PR itself. This repo is a mirror and not for development.
