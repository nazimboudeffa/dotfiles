# Installation

Basically I have made sh script to make everything automatically but, I have some issues

I use Ubuntu Server, let's try by hand first before automating the installation

Suppose your default user is `ubuntu`

## OH MY ZSH

Install zsh

`sudo apt install zsh`

Go to https://ohmyz.sh/ and click on Install oh-my-zsh

Then you'll have this command because I use Ubuntu Server and that curl is not installed by default

`sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"`

Do you want to change your default shell to zsh, type Y and press enter

Now you can change the ohmyzsh theme

Go to https://github.com/ohmyzsh/ohmyzsh/wiki/Themes and choose your theme by following the steps

Let's peek aussiegeek atm

All you have to do is open `~/.zshrc` and add `ZSH_THEME=aussiegeek`

## VIM

```
sudo mkdir -p .vim/bundle
cd .vim/bundle
sudo git clone git://github.com/VundleVim/Vundle.vim.git
vim +PluginInstall +qall <-- E492
```

TODO: FIX ERROR E492
