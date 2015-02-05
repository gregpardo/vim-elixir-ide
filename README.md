# vim-elixir-ide
Get started with Elixir development in minutes!

This repository is a modified version of [farazdagi's original vim-go-ide](https://github.com/farazdagi/vim-go-ide)

I simply modified some things for elixir development.

### 1. Install runtime:

    git clone git@github.com:gregpardo/vim-elixir-ide.git ~/.vim_elixir_runtime
    sh ~/.vim_elixir_runtime/bin/install

**NOTE:** You system's Vim configuration will NOT be changed i.e. it is safe to install.

### 2. Run your newly installed Vim configuration:

Remember that your system's Vim config files remain untouched? During installation `.vimrc.elixir` is created. Let's use it:

    vim -u ~/.vimrc.elixir

And btw, nothing prevents you from creation of a handy alias in your `.zshrc`:

    alias vimelixir='vim -u ~/.vimrc.elixir'

### 3. Mix tasks:

Included in the vim plugins is [vim-mix](https://github.com/mattreduce/vim-mix). Commands are mapped as follows. The default leader key is ','.

	,md - Mix command (runs default mix command)
	,mc - Clean
	,mm - Compile
	,md - Mix list dependencies
	,mdc - Mix dependency clean
	,mdm - Mix dependency compile
	,mdg - Mix dependency get
	,mdu - Mix dependency update
	,mt - Mix test

### 4. Color scheme support 
You can use any supported colorscheme from this [list](https://github.com/flazz/vim-colorschemes/tree/master/colors)

The default is molokai with dark background. To use a color scheme pass the scheme to the install command.

    ~/.vim_elixir_runtime/bin/install railscasts dark

### 5. End-result:

![Screenshot](https://raw.githubusercontent.com/gregpardo/vim-elixir-ide/master/screenshot.png)

Yep, that's it!
