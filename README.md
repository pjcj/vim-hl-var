# Vim plugin to highlight variables in Perl

This Vim plugin will highlight all instances of the Perl variable under the
cursor.  It is a fork of Sandeep.c.r's plugin to do the same for PHP.

![Imgur](http://i.imgur.com/f9N2asZ.gif)

(This is from Sandeep's README, I am too lazy to redo it with Perl code.)

Perl variables, of all types, will be highlighted, as will methods.

## Installation

If you are using a package manager such as *Vundle* or *Pathogen*, this plugin
should be installed in the standard manner.  If you are not (why not?), you
could just copy *hl-var.vim* into your *~/.vim/plugins* directory.

## Configuration

You can customise the highlighting applied by this plugin by using the *hlvarhl*
global variable. This can be set in your *.vimrc* file:

`let g:hlvarhl="ctermbg=black ctermfg=red guifg=#ff0000 guibg=#000000 gui=bold"`

If you don't want the variable under cursor to be highlighted, you can disable
it by setting variable *g:hlvarcurrent* to 1.

`let g:hlvarcurrent = 1`

## Licence

This code is released under the MIT licence, as is Sandeep's original code.
Forked from Sandeep's [repository](https://bitbucket.org/sras/vawa), with his
blessing.
