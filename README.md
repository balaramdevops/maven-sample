# maven-sample
maven
To clone the repository
git clone https://github.com/balaramdevops/maven-sample.git

Build Artifact:
cd maven-sample
mvn clean install

This will create a war file in the target folder.

To run ansible playbook, go to ansible folder and run
ansible-playbook -i hosts middleware.yaml

Note: Make sure you have proper ipaddress specified in the hosts file and have ssh keys configured and proper privileges setup for the "remote_user"

This playbook will install jboss and deploy the war file
Access the app: http://<ListenAddress>:8080/mavenDemo
  
  
