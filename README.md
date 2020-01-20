# Chromebook Linux Setup
```
sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install ruby patchelf -y
sh -c "$(curl -fsSL https://raw.githubusercontent.com/Linuxbrew/install/master/install.sh)"
test -d ~/.linuxbrew && eval $(~/.linuxbrew/bin/brew shellenv)
test -d /home/linuxbrew/.linuxbrew && eval $(/home/linuxbrew/.linuxbrew/bin/brew shellenv)
test -r ~/.bash_profile && echo "eval \$($(brew --prefix)/bin/brew shellenv)" >>~/.bash_profile
echo "eval \$($(brew --prefix)/bin/brew shellenv)" >>~/.profile
brew install hello
hello
brew install openssh
brew install python3
brew install vim
# copy SSH keys from google drive to .ssh
```
