# ambiente

# curl

sudo apt update && sudo apt upgrade

sudo apt install curl

# git 

sudo apt-get install git-all
# Docker-compose

sudo apt-get update

sudo apt-get install curl
sudo apt-get install gnupg
sudo apt-get install ca-certificates
sudo apt-get install lsb-release
### Download the docker gpg file to Ubuntu
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

### Add Docker and docker compose support to the Ubuntu's packages list
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-pluginsudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-pluginlinux/ubuntu   $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin

sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

# terminator
sudo add-apt-repository ppa:gnome-terminator/nightly

sudo apt-get update

sudo apt-get install terminator

sudo apt-get install zsh

sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"

# Chrome

wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

sudo apt install ./google-chrome-stable_current_amd64.deb

# PGadmin 4
#Adiciona uma chave
curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add

#Cria repositório para o arquivo e atualiza
sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'

#Instala o pgadmin4 
sudo apt install pgadmin4

#Instala o pgadmin4 para usar no desktop
sudo apt install pgadmin4-desktop

#Instala o pgadmin4 para usar no browser
sudo apt install pgadmin4-web 

# conectar via ssh

ssh-keygen -t rsa

cat ~/.ssh/id_rsa.pub 

# after clone the projects use 

sudo chown -R $USER:$USER .