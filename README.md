sudo apt install openjdk-11-jre-headless  --> pre req for jenkins
sudo apt install git

Jenkins Installation
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update
IF Error run the below command with the key provided in the error
	sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 9B7D32F2D50582E6
sudo apt update
sudo apt install jenkins

admin/password

git conn setup
ssh-keygen -t rsa -b 4096 -C "balaji22827@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
cat ~/.ssh/id_rsa.pub

copy above key on gituhb ssh UI
