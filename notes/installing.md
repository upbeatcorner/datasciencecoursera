Try installing Python by normal means. If you don't know your password,
you'll have trouble running `sudo` commands, so you'll have to install
things inside your `$HOME` directory. To do that, run this.

    easy_install -d "$HOME/python" virtualenv
    "$HOME/python/virtualenv" "$HOME/env"

copy this to your `~/.profile`,

    alias easy_install="easy_install -d $HOME/python"
    export PATH=$PATH:$HOME/python
    . $HOME/env/bin/activate

and open a new terminal.
