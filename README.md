# neovim-init-vim
Personal customized init.vim for [Neovim](https://neovim.io/).

````

set tabstop=4        " The width of a TAB is set to 4.
                     " Still it is a \t. It is just that
                     " Vim will interpret it to be having
                     " a width of 4.
set shiftwidth=4     " Indents will have a width of 4.
set softtabstop=4    " Sets the number of columns for a TAB.
set expandtab        " Expand TABs to spaces.
set nowrap           " do not automatically wrap on load
set formatoptions-=t " do not automatically wrap text when typing
set nu               " Sets linenumbers

" vimwiki
let wiki_1 = {}
let wiki_1.path = '~/Stack/Wiki'
let wiki_1.template_path = '~/Stack/Wiki/templates'
let wiki_1.template_default = 'default'
let wiki_1.template_ext = '.html'
let wiki_1.ext = '.wiki'

let g:vimwiki_list = [wiki_1]
let g:vimwiki_use_mouse=1

let g:netrw_banner       = 0
let g:netrw_winsize      = 25
let g:netrw_liststyle    = 3
let g:netrw_browse_split = 4

set mouse+=a

nnoremap <C-E> :Vexplore<enter>
nnoremap <C-F> :VimwikiSearch<space>/\c
nnoremap <C-N> :lnext<enter>

highlight VimwikiHeader1 ctermfg=27
highlight VimwikiHeader2 ctermfg=27
highlight VimwikiPre ctermfg=68
highlight LineNr ctermfg=grey

````
