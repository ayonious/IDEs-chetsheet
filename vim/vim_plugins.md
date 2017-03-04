Plugin manager is something that helps to install other plugins. Best plugin manager I think for vim is
`VBundle`


#Install Vbundle
```
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

Now add this in .vimrc file
```
set nocompatible              " be iMproved, required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()

" let Vundle manage Vundle, required
Plugin 'gmarik/Vundle.vim'

" more Plugin commands
" ...
call vundle#end()            " required
filetype plugin indent on    " required
```


# Install NERDTree vim pluging (using Vbundle)

Your .vimrc file will looks like this
```
syntax on
set number
set backspace=indent,eol,start
" http://vi.stackexchange.com/questions/2162/why-doesnt-the-backspace-key-work-in-insert-mode

set nocompatible              " required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()

" alternatively, pass a path where Vundle should install plugins
call vundle#begin('~/some/path/here')


" 1.let Vundle manage Vundle, required
Plugin 'gmarik/Vundle.vim'

" 2.nerdtree plugin
Plugin 'scrooloose/nerdtree'


" Add all your plugins here (note older versions of Vundle used Bundle instead of Plugin)
" All of your Plugins must be added before the following line
call vundle#end()            " required
filetype plugin indent on    " required
```


Now install the plugin from vim
```
<esc> 
:PluginInstall
after the plugin has been installed close the extra splitted window by :bdelete
```