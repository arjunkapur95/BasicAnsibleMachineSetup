# BasicAnsibleMachineSetup
List of steps for Setting up ansible on a Redhat Image / same steps apply for Redhat on AWS
* sudo subcription-manager register
* sudo subcription-manager subscribe

# Refrences For Installing
* Ansible https://developers.redhat.com/blog/2016/09/02/how-to-install-and-configure-ansible-on-rhel/ 
* Apache  https://access.redhat.com/discussions/917293 
* Chrome  https://access.redhat.com/discussions/917293 
* Installing Node https://nodejs.org/en/download/package-manager/
* Disable Selenix https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/security-enhanced_linux/sect-security-enhanced_linux-enabling_and_disabling_selinux-disabling_selinux 

# Run Apache as an Admin User
* Edit this file /etc/httpd/conf/httpd.conf 
    Add Timeout 3400 under server root 
    Add User as arjun 
    Add Group as arjun 

* Add Timeout and change group and user variables here to (arjun for user and arjun for group) 
* Finally run httpd -t (This is a syntax check) 

Now Clone the Angular Project (https://gitlab.com/AnsibleSetup/AnsibleUIApp.git) to the var/www/html location and run npm install 

After that run ng build following which you can copy all the files from destination folder to /var/www/html location 

Note also copy the assests folder. 
