
# 效果

![iterm2.gif](images/iterm2.gif)

# 下载并安装 iterm2

[Iterm2 官网](https://www.iterm2.com/)  

1. 下载后加入应用程序  

2. 给予 完全访问权限

# 切换 iterm2 的主题

[dracula theme](https://draculatheme.com/iterm/)
```
$ git clone https://github.com/dracula/iterm.git

1. iTerm2 > Preferences > Profiles > Colors Tab
2. Open the Color Presets... drop-down in the bottom right corner
3. Select Import... from the list
4. Select the Dracula.itermcolors file
5. Select the Dracula from Color Presets...
```

# 安装 oh-my-zsh



[oh-my-zsh github](https://github.com/robbyrussell/oh-my-zsh)  
```
# 安装在根目录
cd ~
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

# 安装 oh-my-zsh 主题

[spaceship-prompt](https://github.com/denysdovhan/spaceship-prompt)  
```
git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"

ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

Set ZSH_THEME="spaceship" in your .zshrc
vim ~/.zshrc
```

# 安装 FiraCode 字体

[FiraCode github](https://github.com/tonsky/FiraCode)  

下载后拖到mac字体库  
iterm2 中设置字体

# 切换shell
```
chsh -s /bin/zsh
chsh -s /bin/bash
```

# 安装自动提示
[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)  
```
Clone this repository into $ZSH_CUSTOM/plugins (by default ~/.oh-my-zsh/custom/plugins)  

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions


Add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):  

plugins=(zsh-autosuggestions)  
```

