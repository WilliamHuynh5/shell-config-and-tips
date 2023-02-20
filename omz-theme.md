## Changing the theme of `oh-my-zsh` 🎨
1. In the **WSL Terminal** type the following command and press **Enter** to install the PowerLevel10k theme.
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
```
2. Edit the `.zshrc` file to change the theme with:
```
nano ~/.zshrc
```
3. Change the `ZSH_THEME` to `"powerlevel10k/powerlevel10k"` like so:
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
![Terminal](/assets/img-5.png "img-5")

> Note: Lines that start with `#` are comments and will be ignored by `zsh`.

4. Save the file by pressing the following keys:
> This attempts to exit NANO
```
ctrl + x 
```
> Selecting 'y' saves your file
```
y 
```
> Pressing Enter confirms your choice and closes NANO
```
Enter
```

5. Close WSL and open it again.

> There are **lots more themes** for you to browse [here](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)!

### ✅ Now it's time to install **PowerLevel10k** fonts! 😎 To get started, click [here](pl10k-install.md)!