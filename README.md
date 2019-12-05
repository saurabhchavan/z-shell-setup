# z-shell-setup

### Oh My Zsh Installtion Steps ###

**Prerequisites**
- [Zsh](https://www.zsh.org/) should be installed (v4.3.9 or more recent). If not pre-installed (run zsh --version to confirm), check the following instructions here: [Installing ZSH](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)
- curl or wget should be installed
- git should be installed

**Oh My Zsh Installation**

- Open terminal or command prompt and type one of the following command:

  ***Via CURL***
  - sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

  ***Via WGET***
  - sh -c "$(wget -O- https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
- Once installtion is done you can configure the theme and font styel to be used in Oh My Zsh.

**Fonts Setup**
- Open terminal or command prompt and type the following commands:
 - git clone https://github.com/powerline/fonts.git
 - cd fonts
 - ./install.sh
 - cd ..
 - rm -rf fonts
- This will install Powerline Fonts

**Theme Setup**
- To install a custom theme and use it type the following command in terminal or command prompt:
- If on OSX, you will have to make the .files and .folders visible on your system. To do that run the following command:
 - defaults write com.apple.finder AppleShowAllFiles YES
 - Once the command has been executed hold the alt/option button and right click on the finder and relaunch it. Once the finder is relaunced you will be abale to see all the .files and .folders on your system.
- Go to the root directory where you have installed oh my zsh and type the following command:
 - cd .oh-my-zsh
 - cd custom
 - cd themes
 - git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k\
 - /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
 - brew install python
 - pip install --user git+git://github.com/powerline/powerline
  - If on running the above command you get this error "bash: pip: command not found" then you need to install pip before you execute the pip install command.
  - To install pip run sudo easy_install pip and then again run the above command.
- Once the theme installtion has been done type open ~/.zshrc
- A file will open where you have to mention the theme name to be used which in our case is "powerlevel9k".
- Search for a line ZSH_THEME="" and add theme name like this ZSH_THEME="powerlevel9k/powerlevel9k"
- Save and close the file.
- Theme setup is complete now.

**Make Oh My Zsh default**
- Run the followinf comand to make Oh My Zsh as default:
 - chsh -s /bin/zsh
 - restart your terminal.

