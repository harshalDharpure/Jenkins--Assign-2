#Jenkins CI-CD Deployment 

Commands to configure the Jenkins for CI-CD pipelines

1) we have to make a 3 Aws Instances in that we have to select the the Ubuntu machine , then we are using the t2-Micro. after that we
2) have to create a key-pair for the jenkins.
3) then we have to allow the Inbound traffic and the Outbound traffic to allow the traffic
4) then we have to create a Instance.

Important Commands to configure the Jenkins,

1) sudo apt-get update
2) we have to create a bash file in which we have to paste the below commands and also we have to write the -y after the install jenkins commands

3) sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins

4) sudo apt install fontconfig openjdk-17-jre
5) sudo systemctl enable jenkins
6) sudo systemctl start jenkins
7) sudo systemctl status jenkins
8) Always jenkins start at 8080 port Number
9) sudo cat /var/lib/jenkins/secrets/initialAdminPassword
10) java --version
11) start the jenkins server and configured the Master and slave Architecture  
