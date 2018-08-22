Tools That I may needs to setup in future.

--> Opengrok on Linux or Windows Machine.
--> tmux 
--> vim with ctags and taglists.
--> git  1991MANISH/Manish123#
--> cscope

Ctrl+] - go to definition
Ctrl+T - Jump back from the definition.
Ctrl+W Ctrl+] - Open the definition in a horizontal split

Add these lines in vimrc
map <C-\> :tab split<CR>:exec("tag ".expand("<cword>"))<CR>
map <A-]> :vsp <CR>:exec("tag ".expand("<cword>"))<CR>

Ctrl+\ - Open the definition in a new tab
Alt+] - Open the definition in a vertical split

After the tags are generated. You can use the following keys to tag into and tag out of functions:

Ctrl+Left MouseClick - Go to definition
Ctrl+Right MouseClick - Jump back from definition

]c               - advance to the next block with differences
[c               - reverse search for the previous block with differences
do (diff obtain) - bring changes from the other file to the current file
dp (diff put)    - send changes from the current file to the other file
zo               - unfold/unhide text
zc               - refold/rehide text
zr               - unfold both files completely
zm               - fold both files completely

do - Get changes from other window into the current window.

dp - Put the changes from current window into the other window.

]c - Jump to the next change.

[c - Jump to the previous change.

zo - open folded lines.

zc - close folded lines.

Ctrlww - change window.

:only | wq - quit other windows, write and quit.
