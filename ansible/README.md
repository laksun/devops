Ansible installation and configuration on Ubuntu 14.04 (master), centos 7.2 (client)

Ubuntu (master):

 a. Update the ubuntu	   :  sudo apt-get update
 
	   b. sudo apt-get install software-properties-common
	   
	   c. sudo apt-add-repository --yes  ppa:ansible/ansible
	   
	   d. sudo apt-get install ansible
	   
	   e. ssh-keygen
	   
	   f. chmod 600 .ssh/id_rsa.pub
	   
	   g. sudo service ssh restart
	   
	   h. sudo apt-get install tree
	   
	   Update ansible:
	   
	        sudo apt-get install python-pip python-dev
		
		sudo apt-get update && sudo apt-get install ansible
		
		ansible --version
      
Centos (client):

    a.  nano .ssh/authorized_keys
    
	      copy the content from the server id_rsa.pub into the .authorized_keys file
		
		b. service sshd restart
		
		c. yum -y update
    
