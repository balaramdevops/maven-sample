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

Note: Make sure you have proper ipaddress specified in the hosts file

This playbook will install jboss and deploy the war file that 
Access the app:Screen Shot 2020-04-13 at 11.53.38 AM
http://<ListenAddress>:8080/mavenDemo
  
  
