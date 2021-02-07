# Skrypt Stawiania systemu
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update; sudo apt-get install -y sublime-text git-all terminology curl golang-go python3 python-is-python3 cmake zsh tmux brave-browser
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)";git clone https://github.com/pragmaticivan/dotfiles.git ~/.dotfiles
cd ~/.dotfiles;./script/bootstrap



################## ls kolor dodaj alias 
sudo apt-get install libhttp-parser2.1
wget https://github.com/ogham/exa/releases/download/v0.9.0/exa-linux-x86_64-0.9.0.zip
unzip exa-linux-x86_64-0.9.0.zip
sudo mv exa-linux-x86_64 /usr/local/bin/
################### alias ls="/usr/local/bin//exa-linux-x86_64"
echo "alias ls='exa -l'" >> ~/.bash_aliases

chwila dzisiejsza not pisanie skryptów beda resy itd musze przygotowac srodowisko ktore odpala all na raz troche to zajmie i han w dzisiejsze manewry
