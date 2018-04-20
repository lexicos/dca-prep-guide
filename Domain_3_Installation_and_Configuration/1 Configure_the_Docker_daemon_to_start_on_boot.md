# Configure the Docker daemon to start on boot

## Official Docker Documentation
[Configure Docker to start on boot](https://docs.docker.com/engine/installation/linux/linux-postinstall//)  

## Add docker user group and assign as local user
sudo groupadd docker
sudo usermod -aG docker $USER

## Test it works
docker run hello-world

$ sudo chown "$USER":"$USER" /home/"$USER"/.docker -R
$ sudo chmod g+rwx "/home/$USER/.docker" -R

## RHEL, CentOS, Fedora, Ubuntu 16.04 and higher)
sudo systemctl enable docker
OR
sudo systemctl enable docker.service
sudo systemctl start docker.service

sudo systemctl disable docker

## Ubuntu 14.10 and below use upstart which is automatically configured
sudo chkconfig docker on

## Windows ### 
TBC cant find that much on the forums best to test


