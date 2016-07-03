# foldsearches.vim

Forked from [Damian-Conway-s-Vim-Setup](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup/blob/master/plugin/foldsearches.vim).

### Rationale

Display all search results and folds the rest of the buffer.
Forked just to be able to use it as a plugin with VIM plugin managers like [ pathogen
](https://github.com/tpope/vim-pathogen), [ vundle ](https://github.com/VundleVim/Vundle.vim), [ vim-plug
](https://github.com/junegunn/vim-plug) etc.

### Usage

From Damian's .vimrc:

```viml
"=====[ Search folding ]=====================

" Don't start new buffers folded
set foldlevelstart=99

" Highlight folds
highlight Folded  ctermfg=cyan ctermbg=black

" Toggle on and off...
nmap <silent> <expr>  zz  FS_ToggleFoldAroundSearch({'context':1})
```

`context` determines how many lines around the `search term` will be visible between folds.

### Licence, disclaimer as from Damian's repo

*Totally unsupported.*

---------

Copyright (c) 2011-2016, Damian Conway. All rights reserved.

This is free software. It may be used, redistributed
and/or modified under the terms of the Perl Artistic License
(see http://www.perl.com/perl/misc/Artistic.html)


DISCLAIMER OF WARRANTY

BECAUSE THIS SOFTWARE IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
FOR THE SOFTWARE, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN
OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
PROVIDE THE SOFTWARE "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER
EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE
ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE SOFTWARE IS WITH
YOU. SHOULD THE SOFTWARE PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL
NECESSARY SERVICING, REPAIR, OR CORRECTION.

IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
REDISTRIBUTE THE SOFTWARE AS PERMITTED BY THE ABOVE LICENCE, BE
LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL,
OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE
THE SOFTWARE (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
FAILURE OF THE SOFTWARE TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
SUCH DAMAGES.

