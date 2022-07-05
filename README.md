# ambiente

# curl

sudo apt update && sudo apt upgrade

sudo apt install curl

# git 

sudo apt-get install git-all
# Docker-compose

sudo apt-get update

 sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release

    sudo mkdir -p /etc/apt/keyrings

 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

 echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin

sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

# terminator
sudo add-apt-repository ppa:gnome-terminator/nightly

sudo apt-get update

sudo apt-get install terminator

sudo apt-get install zsh

# Chrome

wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

sudo apt install ./google-chrome-stable_current_amd64.deb

# conectar via ssh

ssh-keygen -t rsa

cat .ssh/id_rsa.pub 

# after clone the projects use 

sudo chown -R $USER:$USER .