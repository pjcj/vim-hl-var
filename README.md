# Vim plugin to highlight variables in Perl

This Vim plugin will highlight all instances of the Perl variable under the
cursor.  It is a fork of Sandeep.c.r's plugin to do the same for PHP.

![Imgur](https://i.imgur.com/yBnFrby.gif)

(Image credit: [Ovid](https://github.com/ovid))

Perl variables, of all types, will be highlighted, as will methods.

## Installation

If you are using a package manager such as *Vundle* or *Pathogen*, this plugin
should be installed in the standard manner.  If you are not (why not?), you
could just copy *hl-var.vim* into your *~/.vim/plugins* directory.

Requires Vim version 7.3 or later.

## Configuration

The variables will be highlighted after you have not performed any action for a
certain length of time.  That time is controlled by the *updatetime* setting.
(See `:help updatetime`.) The default value is 4000, which is four seconds.
That value is too large for this plugin, so I recommend adjusting it to 500,
which is half a second.  You can experiment with the value which works best for
you.

`set updatetime=500`

You can customise the highlighting applied by this plugin by using the *hlvarhl*
global variable. This can be set in your *.vimrc* file:

`let g:hlvarhl="ctermbg=black ctermfg=red guifg=#ff0000 guibg=#000000 gui=bold"`

If you don't want the variable under cursor to be highlighted, you can disable
it by setting variable *g:hlvarcurrent* to 1.

`let g:hlvarcurrent = 1`

## Licence

This code is released under the MIT licence, as is Sandeep's original code.  See
*hl-var.vim* for the full licence.

## Authors

This version was forked from Sandeep's
[repository](https://bitbucket.org/sras/vawa), with his blessing.  Curtis "Ovid"
Poe hacked it to support Perl.  It is currently being maintained by Paul
Johnson.
