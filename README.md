# docker-installation
docker installations for servers


#amazon linux2 AMI:
sudo yum install update
sudo yum install docker -y
docker --version
systemctl start docker --> chkconfig docker on --> #check the docker status --> systemctl status docker
#git installation: yum install git -y
#Install docker-compose:
Copy the appropriate docker-compose binary from GitHub:

sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose

NOTE: to get the latest version (thanks @spodnet): sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose

Fix permissions after download:

sudo chmod +x /usr/local/bin/docker-compose

Verify success:

docker-compose version

