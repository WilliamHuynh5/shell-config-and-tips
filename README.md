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

```
sudo apt-get install zsh
```

![Winver Example](/assets/img-1.png "img-1")

## Installing oh-my-zsh
1. Make sure you have `git` installed. In the **WSL Terminal** type the following command and press **Enter**

```
sudo apt-get install git
```

2. Install `oh-my-zsh`. In the **WSL Terminal** type the following command and press **Enter**

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

![Winver Example](/assets/img-2.png "img-2")

## Making ZSH our default shell

1. In the **WSL Terminal** type the following command and press **Enter**

```
chsh -s $(which zsh)
```

> You may be prompted to enter in your password. If the prompt appears, **type your password** and press **Enter**.

2. Close WSL and reopen it again. 

## Installing Powerline10k Fonts
1. Make sure `git` is installed on your Windows machine (**not WSL**).
> You can download `git` for Windows [here](https://git-scm.com/download/win).

2. Open **Start** on Windows
3. Search for **terminal**
![Terminal](/assets/img-3.png "img-3")
4. In the **Windows Terminal** type the following command and press **Enter**
```
git clone https://github.com/powerline/fonts.git
```
![Terminal](/assets/img-4.png "img-4")
5. In the same  **Windows Terminal**, navigate to the newly cloned `fonts` directory by typing the following command and pressing **Enter**
```
cd fonts
```
6. In the same  **Windows Terminal**, install the fonts by typing the following command and pressing **Enter**
```
.\install.ps1
```

## Changing the theme of `oh-my-zsh`
1. Enter the following command and press **Enter** to edit the `.zshrc` file to change the theme.
2. Change the `ZSH_THEME` to `"agnoster"`
```
ZSH_THEME="agnoster"
```
![Terminal](/assets/img-5.png "img-5")

> Note: Lines that start with `#` are comments and will be ignored by `zsh`.

3. Close WSL and open it again.

## Changing the font to `PowerLevel10k`
When you reopen WSL you might notice your terminal looks broken; something like this:
![Terminal](/assets/img-6.png "img-6")
This is because we haven't loaded the PowerLevel10k fonts for use in WSL. 

1. Right-click on the border of the WSL application to open the context menu.
![Terminal](/assets/img-7.png "img-7")
2. Click on `Properties`
3. Click on `Fonts`
4. Select `Ubuntu Mono derivative Powerline` in the fonts menu
![Terminal](/assets/img-8.png "img-8")

And voila! Your terminal should be spice up!
![Terminal](/assets/img-9.png "img-9")