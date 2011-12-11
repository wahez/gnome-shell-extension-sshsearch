Ssh Search Provider
=====================
A gnome-shell extension which searches the ssh config file and
provides the found ssh connections in your shell overview.

So you need a ~/.ssh/config file to use this extensions. It parses
the config file and search for the strings after the "Host" setting.

### Installation
* copy or link the folder "ssh-search-provider@gnome-shell-extensions.brot.github.com" to ~/.local/share/gnome-shell/extensions
* enable extension (e.g. via gnome-tweak-tool)

### Selecting Your preferred Terminal Application
At the moment it isn't possible to configure your preferred terminal application. 
The reason is that gnome-shell in the current stable version (3.2) don't easily allow 
extensions to use a extension specific gsettings schema.
But this should be possible with the next stable gnome-shell version (3.4)

At the moment you could change the default terminal app if you override the setting 
directly in the source file:
~/.local/share/gnome-shell/extensions/ssh-search-provider@gnome-shell-extensions.brot.github.com/extension.js
There you could change the following line to your needs. This is the default setting:

    const SSHSEARCH_TERMINAL_APP = 'gnome-terminal';
    
For example you could change this to 

    const SSHSEARCH_TERMINAL_APP = 'terminator';
    
if you would like to use Terminator as your terminal application

### License
Copyright (c) 2011 Bernd Schlapsi <brot@gmx.info>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
