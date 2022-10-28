# Development_Environment_Node_Mongo

Welcome to my Development-Environment-Node-MongoDB application Repository

I have included my Node/MongoDB application along with a few other things to make it quick and easy for 
you to set up a virtual machine environment on your computer and be able to access the application and have the example app running on your web browser.

First you will need to have a couple dependencies installed on your computer which are:
1. Vagrant (hashicorp)
2. VirtualBox (Oracle Vm) or VMWare if you are using an M1 chip.

This repo includes:
1. an app folder that contains the Node/MongoDB files and tests for the application code.
2. an env folder which contains a nodeapp and a mongodb folder, each containing a script.sh file that will provision the virtual machine to run the application
and a conf file to be used for configuration in the scripts.
3. a Vagrantfile that will configure and initialize the virtual machine.

Once you have those installed you can clone this repo to your computer in whatever file destination you decide.

Everything should be set up and ready for you to run a simple command to start your virtual machine. 
(Be sure to go into the VagrantFile and comment out the appropriate Vagrant.configure block in accordance to your Operating System).
Open up the terminal to the repo path and run the command: vagrant up

This will start up the virtual machine and the provisioning script.sh that is included should install and neccesary dependecies for your application to run. 

Once the the vagrant up command is completed you should then be able to go to your browser and enter http://nology.training:3002/cicd to view the
example app running.
