# MacEnv

## Introduction
This repo is a Guide to setting up a dev environment on OS X  

## Browsers

[Chrome](https://www.google.com/chrome/browser/desktop/index.html)  
[Firefox](https://www.mozilla.org/en-US/firefox/desktop/)  
[Opera](http://www.opera.com/download) - Free VPN built in

## Browser Extensions

[LastPass](https://www.lastpass.com/) - Password manager  
[Grammarly](https://www.grammarly.com/) - Spell check everywhere  
[Honey](https://www.joinhoney.com/) - Search for coupons upon checkout  
[Pushbullet](https://www.pushbullet.com/) - Push mobile notifications to desktop notifications  
[Reddit Enhancement Suite](https://redditenhancementsuite.com/) - Reddit power tools  
[Adblock Plus (chrome)](https://chrome.google.com/webstore/detail/adblock-plus/cfhdojbkjhnklbpkdaibdccddilifddb)  
[BetterTTV](https://nightdev.com/betterttv/) - Twitch.tv enhancments  
[Ghostery](https://www.ghostery.com/) - Remove internet tracking  
[Postman](https://www.getpostman.com/) - REST API requests  
[React Dev Tools (Chrome)](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en)  
[Hola](https://hola.org/) - Free basic browser vpn  

## Mac Apps

[Flux](https://justgetflux.com/) - Alternative to night shift  
[Alfred](https://www.alfredapp.com/) - Alternative to spotlight  
[Spectacle](https://www.spectacleapp.com/) - Resize windows with keyboard shortcuts  
[Divvy](http://mizage.com/divvy/) - Resize windows to custom grid size  
[BetterTouchTool](https://www.boastr.net/) - Map custom keyboard/mouse/trackpad shortcuts to actions  


## In Progress

chrome
Firefox
Firefox nightly
Chrome canary
Opera


Sign into last pass to get google chrome login 
Mac App Store, update all apps including OS X

Mac App Store
	X Code
	Memory Clean
	The Unarchiver

Home brew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"


Iterm2
Oh my zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

powerline fonts
git clone https://github.com/powerline/fonts.git --depth=1
cd fonts
./install.sh
cd ..
rm -rf fonts


Git clone https://github.com/wesbos/Cobalt2-iterm.git
Cd Cobalt2-iterm
Cp cobalt2.zsh-theme ~/.oh-my-zsh/themes/

curl -O “https://bootstrap.pypa.io/get-pip.py”
sudo python get-pip.py


pip install --user powerline-status


iTerm2 > Preferences > Profiles > Colors > Color Presets… dropdown > Import > Cobalt2-iterm/cobalt2.itermcolors

Select ‘cobalt’ from dropdown

Iterm2 dark theme:
Iterm2 > Preferences > Appearance > Theme: Dark

iTerm2 > Preferences > Profiles > Text > Under Font, Change font to ‘Inconsolata for Powerline’ 

Also enable checkbox: Use a different font for non-ASCII text
New Options appear. Under Non-ASCII Font, Change font to ‘Inconsolata for Powerline’

chsh -s /bin/bash
OR chsh -s $(which zsh).


Quit then reopen iterm2

Source ~/.zshrc




Adding ll shortcut

vim ~/.bash_profile
alias ll='ls -lGaf'


Update git
Brew install git
export PATH="/usr/local/bin:${PATH}"
source ~/.bash_profile

Should no longer be using default apple git

git config --global user.name "Your Name Here"
git config --global user.email "your_email@youremail.com"


Adding Github ssh key

Mkdir ~/.ssh
Cd ~/.ssh
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
Enter, enter a passphrase

Vim ~/.ssh/config

Host *
 AddKeysToAgent yes
 UseKeychain yes
 IdentityFile ~/.ssh/id_rsa

ssh-add -K ~/.ssh/id_rsa
pbcopy < ~/.ssh/id_rsa.pub

https://github.com/settings/keys
New SSH key > paste key > save


Adding global git ignores

git config --global core.excludesfile ~/.gitignore
curl https://raw.githubusercontent.com/github/gitignore/master/Global/macOS.gitignore -o ~/.gitignore

Create GitHub working directory
Mkdir ~/Github

Change default Mac location
Mkdir ~/Screenshots
defaults write com.apple.screencapture location /Users/Dennis/Screenshots/

Add Screenshots and Github folders to finder favourites
Open ~/
Drag the two folders to the side bar of finder (Favourites) 



Text editors
Download vscode https://code.visualstudio.com

Set ‘code’ in path
Command + shift + P

Shell Command: install ‘code’ command in PATH


Download sublime3 https://www.sublimetext.com/
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin

Flux instead of night shift
https://justgetflux.com

Alfred
https://www.alfredapp.com/

Launch Alfred instead of spotlight when pressing default command + space:
System preferences > keyboard > shortcuts > set ‘Show Spotlight search’ to option + space
Open Alfred settings and set Alfred hotkey to command + space

Set Alfred theme to dark
Alfred preferences > appearance > Alfred Dark 


Set key repeat to fast
System preferences > keyborad > keyboard > set Key Repeat to fast, set Delay Until Repeat to short
While in here, enable ‘Show keyboard and emoji viewers in menu bar’


Change keyboard modifiers
System preferences > keyborad > keyboard > Modifier Keys button
Caps Lock -> Control
Control -> Command

Enable keyboard access to windows and dialogs
System preferences > keyborad > shortcuts > set Full Keyboard Access to ‘All controls’


Spotify https://www.spotify.com

Teamviewer https://www.teamviewer.com/en/

Skype https://www.skype.com/

NodeJS https://nodejs.org/en/

Slack

Mail > Add all email accounts

Spectacle for resizing windows with hotkeys - https://www.spectacleapp.com/