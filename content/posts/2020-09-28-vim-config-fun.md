---
layout: post
title: Vim Config Fun
tags:
- vim
- unix
- config
date: "2020-09-28"
description: "A Vim config"
---

Recently, I've been writing a configuration file for nvim that I believe would be fun. I do use plugins and as I stream every so often, I do have a snippet that I can run a simple command to get, as seen below.

```
" Extra Plugins
call plug#begin('C:\Users\snicf\AppData\Local\nvim\plugs')
Plug 'junegunn/goyo.vim'
Plug 'junegunn/limelight.vim'
Plug 'vim-airline/vim-airline'
Plug 'vim-airline/vim-airline-themes'
Plug 'ctrlpvim/ctrlp.vim'
Plug 'vimwiki/vimwiki'
Plug 'dracula/vim', { 'as': 'dracula' }
Plug 'vim-scripts/AutoComplPop'
Plug 'junegunn/fzf'
call plug#end()

" Aesthetics
colorscheme dracula
let g:airline#extensions#tabline#enabled = 1
let g:airline_theme = 'zenburn'
let g:airline_powerline_fonts = 1
let maplocalleader=";"
let g:limelight_conceal_ctermfg = 240
set noshowmode
set nocompatible
set number
" echom "YAMETE KUDASTOP!"

" Elite Spelling
set spelllang=en
set spellfile=$HOME/.spell.en.utf-8.add
set spell


" Power Keymappings
nnoremap <Leader>h <C-w>h
nnoremap <Leader>j <C-w>j
nnoremap <Leader>k <C-w>k
nnoremap <Leader>l <C-w>l
nnoremap ,twitch :-1read ~\src\twitch.html<CR>6j11l

au BufNewFile,BufRead /*.rasi setf css
filetype plugin on
syntax on
```

This isn't in my dotfiles yet, as I've only been hacking on it on Windows, but soon it shall be. I'll have to pull it down to my Arch laptop. I had to switch from FreeBSD and OpenBSD as the driver support is limited. Also, I've been trying to contribute more to the community. I may not be a hacker, but I am a reader. As such, I've been contributing my books to BookBrainz.
