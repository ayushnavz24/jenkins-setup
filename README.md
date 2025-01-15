# jenkins-setup

install java

sudo apt update

sudo apt install fontconfig openjdk-17-jre

java -version

openjdk version "17.0.13" 2024-10-15
OpenJDK Runtime Environment (build 17.0.13+11-Debian-2)
OpenJDK 64-Bit Server VM (build 17.0.13+11-Debian-2, mixed mode, sharing)

check java install or not command- (java --version)

now install jenkins

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

sudo apt-get update

sudo apt-get install jenkins

systemctl status jenkins

now chenge port 8080 in security group and add
ready to run 
copy public IP and peast in server 
now set admin password
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
now jenkins ready
