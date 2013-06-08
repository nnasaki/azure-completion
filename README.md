azure-completion
==================

SYNOPSIS
-----------
Completion for Windows Azure CLI tool.

Example
--------

    $ azure[tab]
    account  help     portal   service  sql
    config   mobile   sb       site     vm

    $ azure m[tab]
    $ azure mobile[tab]
    onfig     data       job        list       log        scale      show
    create     delete     key        locations  restart    script     table

System Requirements
------------
* bash

zsh is work in process...


Install
------------

    npm install azure-completion -g

    comp-azure  --install >> ~/.bash_profile
    sed -i -e 's/(azure/(comp-azure/' ~/.node-completion/azure
    source ~/.node-completion/azure

Uninstalling
--------------

    npm uninstall azure-completion -g

    rm ~/.node-completion/azure

Delete also text below on `~/.bash_profile`

    #
    # NODE-COMPLETE
    # Custom command line tab completion for Node.js
    #
    shopt -s progcomp
    for f in $(command ls ~/.node-completion); do
      f="$HOME/.node-completion/$f"
      test -f "$f" && . "$f"
    done


License
-----------
(The MIT License)

Copyright (c) 2013 nnasaki https://www.twitter.com/nnasaki

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.