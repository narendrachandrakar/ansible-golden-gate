make sure Ansible Installed 

Download OGG 12.3.0.1.2 for Big Data (Download Link: https://www.oracle.com/technetwork/middleware/goldengate/downloads/index.html )
 


cp OGG_BigData_Linux_x64_12.3.2.1.1.tar into  \ogg_role\final\files

* Note : make sure the same tar file name and keep Inside the files folder

Now run the ansilbe command to install, Only you can run One time, it will install as per requirements, next time its failing becuase of ansible issues

Go to \ogg_role\final , check site.yml should be there.
and Run the command Inside the final folder, change paramter as per system user name i.e here ec2-user


ansible-playbook -vv -U root --extra-vars "username=ec2-user" site.yml