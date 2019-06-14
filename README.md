Please follow these steps carefully! They will allow you to set up an identical development environment.

DO THIS ONE TIME TO SET UP HOST MACHINE

1. Install VirtualBox for your OS. https://www.virtualbox.org/wiki/Downloads
2. Install Vagrant https://www.vagrantup.com/
3. Inside of a directory/folder that will be the parent of the develoment folder on your local machinE do <code>git clone https://github.com/app-mds/frontend-environment.git</code>
4. go into the directory you just pulled down. <code>cd frontend-development</code>
5. Install this to manage symlink issues <code>npm install -g sympm</code>
6. type this to download the proper environment <code>vagrant up</code>
