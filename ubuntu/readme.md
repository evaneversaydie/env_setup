# 
#!/bin/bash
# apt-install which need sudo previleges
sudo_install (){
	sudo apt update
	sudo apt-get install git curl tar -y
	sudo apt-get install zsh vim tmux -y
}

# Check if sudo or not
if [[ "$EUID" -eq 0 ]]; then
	echo "Please do not run as sudo"
	echo "Grant root permission when ask for password later"
	exit 1
fi
sudo_install

# use sudo -u $SUDO_USER to make sure run script/bash as user
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
cp .zshrc ~

# Install oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"