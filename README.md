# Alt mappings in terminal Vim (experimental)

This plugin enables `Alt` key mappings in **terminal** vim.

Now you can do something like this:

    map <M-a> :echo "You just pressed Alt-a!"<CR>
    map <M-X> :echo "Works with uppercase letters."<CR>
    map <M-5> :echo "Numbers are supported too"<CR>
    map <M-$> :echo "as well as characters..."<CR>
    map <M-?> :echo "and more characters..."<CR>
    map <M-~> :echo "and more..."<CR>

### Installation

Use your favorite plugin manager.

- [Pathogen](https://github.com/tpope/vim-pathogen)
  - just `git clone https://github.com/junegunn/vader.vim.git ~/.vim/bundle/vader.vim`
- [Vundle](https://github.com/gmarik/vundle)
  - add `Bundle 'junegunn/vader.vim'` to .vimrc
  - then run `:BundleInstall`
- [NeoBundle](https://github.com/Shougo/neobundle.vim)
  - add `NeoBundle 'junegunn/vader.vim'` to .vimrc
  - then run `:NeoBundleInstall`
- [vim-plug](https://github.com/junegunn/vim-plug)
  - add `Plug 'junegunn/vader.vim'` to .vimrc
  - then run `:PlugInstall`

### Terminal related setup

- OS X Terminal.app: check "Use option as meta key"<br/>
  ![OS X Terminal.app setting](/osx_terminal.png)

- OS X iTerm2, no setup needed

- other?

### Limitations

Mappings for the following keys are (currently?) not possible:

- `Alt-O` (that's `Alt` big o)<br/>
if this one is set, movements arrow keys produce funny characters in insert and
command line mode.
- `Alt->`, `Alt-[` - couldn't find a way to make these one work
- `Alt-space` - when set up, messes up all other mappings

There are more than 90 `Alt` key mappings available, so hopefully you won't
miss the above 4 that are not (jet?) possible.

### Thanks

@tpope for his [rsi.vim](https://github.com/tpope/vim-rsi) plugin, which was an
inspiration for this one.
