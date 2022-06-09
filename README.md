# `tabbed-terminal`

## DESCRIPTION

This script provides terminal emulator multiplexing and focus
for the `xfce4-terminal` or `mate-terminal`.


## USAGE

    $ tabbed-terminal [optional arguments]


### Preferred Applications
In Settings → Preferred Applications → Utilities → Terminal Emulator, put:

    tabbed-terminal --command="%s" --title="%s"


### Launcher
In a Terminal Emulator launcher, just put:

    tabbed-terminal

(The default is: `exo-open --launch TerminalEmulator`.)


### Vim
In `.vimrc`, put:

    command! Terminal :call system("tabbed-terminal --working-directory='".expand("%:p:h")."' &")
    noremap  <silent> <F4> :Terminal<CR>
    vnoremap <silent> <F4> <ESC>:Terminal<CR>
    inoremap <silent> <F4> <ESC>:Terminal<CR>


### SpaceFM
In SpaceFM → View → Preferences → Advanced → Terminal, put:

    tabbed-terminal --title="%D"


## REQUIRES

    awk, pidof, wmctrl


## COPYRIGHT

    Copyright (C) 2015-2022  Serge Y. Stroobandt

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.


## CONTACT

    xdg-open mailto:$(echo c2VyZ2VAc3Ryb29iYW5kdC5jb20K |base64 -d)

