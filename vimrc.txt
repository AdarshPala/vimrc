set number
set background=dark
filetype indent on
colorscheme slate

"set terminal colour mode to 256
set t_Co=256

"allow wildmenu
set wildmenu

"show filename in title bar
set title

"scroll buffer
set scrolloff=8

"better pasting
set paste

"highlight current line
set cursorline

"increase thenumber of lines that can be copied
set viminfo='100,<2000,s1000
autocmd BufRead,BufWritePre *.sh normal gg=G 

"use , as a leader fo when you actually want to cut
let mapleader = "," 
let g:mapleader = ","
"delete without cutting
nnoremap x "_x
nnoremap d "_d
nnoremap D "_D
vnoremap d "_d
nnoremap ,d ""d
nnoremap ,D ""D
vnoremap ,d ""d

"press enter to add a new line without insert mode
nmap <S-Enter> O<Esc>
nmap <CR> o<Esc>

" Highlight search results
set hlsearch

" Makes search act like search in modern browsers
set incsearch 

" Don't redraw while executing macros (good performance config)
set lazyredraw 

" Use spaces instead of tabs
set expandtab

" Be smart when using tabs ;)
set smarttab

" 1 tab == 4 spaces
set shiftwidth=4
set tabstop=4

" Linebreak on 500 characters
set lbr
set tw=500

set ai "Auto indent
set si "Smart indent
set wrap "Wrap lines
