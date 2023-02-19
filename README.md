# Spicing up your shell using ZSH

Welcome to CSESoc Education's guide on Customising your Shell! 

Here you will learn how to customise your WSL shell using tools like `oh-my-zsh`.

> Your terminal before this guide 🤮

![Winver Example](/assets/bad-terminal.png "bad-terminal")

> Your terminal after this guide 🤩

![Winver Example](/assets/cool-terminal.png "cool-terminal")

## What is ZSH & Why use ZSH? 🤔
ZSH is an extended version of Bash, providing the same functionality of Bash, but also with plenty of new features, and support for plugins and themes.

Some notable improvements over Bash include:
- Faster autocompletion
- Tab completion behaves like a drop down 
- Spelling correction

## What is Oh-My-ZSH? 🧠
Oh-my-zsh is an open-source and community driven framework for managing a ZSH configuration. It is the tool that allows us to install functions, plugins and themes onto our ZSH shell.

## Installing ZSH
> If you are on macOS you should have `zsh` installed already

> If you are on Windows, make sure you have followed our WSL Setup Guide before continuing!

1. Open **WSL** *(usually called `Ubuntu on Windows`)*
2. In the **WSL Terminal** type the following command and press **Enter**

```sudo apt-get install zsh```

![Winver Example](/assets/img-1.png "img-1")

## Installing oh-my-zsh
1. Make sure you have `git` installed. In the **WSL Terminal** type the following command and press **Enter**

`sudo apt-get install git`

2. Install `oh-my-zsh`. In the **WSL Terminal** type the following command and press **Enter**

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

![Winver Example](/assets/img-2.png "img-2")

## Making ZSH our default shell

In the **WSL Terminal** type the following command and press **Enter**

`chsh -s $(which zsh)`

> You may be prompted to enter in your password. If the prompt appears, type your password and press **Enter**.
