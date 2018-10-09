# SWITCH FROM BASH TO ZSH
Viveks-MacBook-Air:~ nayan$ which zsh
/bin/zsh

Viveks-MacBook-Air:~ nayan$ chsh -s /bin/zsh
Changing shell for nayan.
Password for nayan: 

Viveks-MacBook-Air:~ nayan$ 

restart terminal

# INSTALL OH MY ZSH
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

restart terminal

# syntax Highlighting Plugin
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
nano ~/.zshrc

add zsh-syntax-highlighting to the plugins section
control+X

source ~/.zshrc (re-read)

#
git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
add zsh-autosuggestions to the plugins section
control+X

source ~/.zshrc (re-read)

# theme and font
1. Install Powerline fonts

$ git clone https://github.com/powerline/fonts.git
$ cd fonts
$ ./install.sh

2. Change the Theme to “agnoster”

$ open ~/.zshrc
Set ZSH_THEME="agnoster" and save the file

Preferences > Profiles > Text > Change Font. I’m choosing “Meslo LG DZ for Powerline” font.
