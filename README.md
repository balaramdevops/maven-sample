# maven-sample:
Clone the repository:
git clone https://github.com/balaramdevops/maven-sample.git

Build Artifact:
cd maven-sample; mvn clean install

This will create a war file in the target folder.

To run ansible playbook, go to ansible folder and run
ansible-playbook -i hosts middleware.yaml

Note: Make sure you have proper ipaddress specified in the hosts file and have ssh keys configured and proper privileges setup for the "remote_user"
If you have multiple hosts, have all the hosts/ip info specified in the hosts file under specific category.
Also there is a way you can create the dynamic inventory for AWS instances, instead of having static hosts defined in the hosts file.
Here is the Documentation on how to set up this.
https://docs.ansible.com/ansible/latest/user_guide/intro_dynamic_inventory.html#inventory-script-example-aws-ec2

This playbook will install jboss and deploy the war file
Access the app: http://ipaddress:8080/mavenDemo


Ansible has very good documentation of modules. Here is the link for the Ansible modules.
https://docs.ansible.com/ansible/latest/modules/modules_by_category.html

Specific to cloud modules:
https://docs.ansible.com/ansible/latest/modules/list_of_cloud_modules.html

Introduction to Ansible modules:
https://docs.ansible.com/ansible/latest/user_guide/modules_intro.html
  
