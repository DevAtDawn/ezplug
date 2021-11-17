# ezplug
neovim plugin to easily add new plugins without editing init.vim

this plugin uses the cmd Ezplug to appened text to a file called plugins.vim, which is sourced inside init.vim

# TLDR
make a file called ~/.config/nvim/plugins.vim and source it inside the init.vim plugins sections 

call plug#begin()

  Plug 'DevAtDawn/ezplug'
  
  source ~/.config/nvim/plugins.vim
  
call plug#end()


# USAGE
to install a plugin, enter the vim command line and type

:Ezplug Plug 'preservim/nerdtree'

or

Ezpg Plug 'DevAtDawn/ezplug'

or for vim-plug you can do

Ezvimplug DevAtDawn/ezplug

# INSTAll
vim-plug example: Plug 'DevAtDawn/ezplug'

create a file called plugins.vim in $HOME/.config/nvim

(same place your init.vim is stored) ex: home/user/.config/nvim/plugins.vim
  
now inside init.vim, source this file by adding the line "source ~/.config/nvim/plugins.vim" to the same section as the previous command

  <details>
  <summary>Vim-Plug</summary>

1. Install Vim-Plug, according to its instructions.
1. Add the following text to your `vimrc`.
```vim
call plug#begin()
  Plug 'DevAtDawn/ezplug'
  source ~/.config/nvim/plugins.vim
call plug#end()
```
1. Restart Vim, and run the `:PlugInstall` statement to install your plugins.
</details>
  
