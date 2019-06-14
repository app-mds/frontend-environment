Please follow these steps carefully! They will allow you to set up an identical development environment.
1. Install VirtualBox for your OS. https://www.virtualbox.org/wiki/Downloads
2. Install Vagrant https://www.vagrantup.com/
3. Inside of a directory/folder that will be the parent of the develoment folder on your local maching do <code>git clone https://github.com/app-mds/frontend-environment.git</code>
4. go into the directory you just pulled down. <code>cd frontend-development</code>
5. curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
** type this to download the proper environment <code>vagrant up</code>

INCLUDED IN VAGRANTFILE
(these items should only need to be done once, when first setting up the VM)

1. Install guest addition plugin by typing this in command line <code>vagrant plugin install vagrant-vbguest</code>

2. Install NVM to manage possible multiple versions of node <code>curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash</code>

3. Install Node (a javascript server side environment) and NPM (a package manager that keeps track of downloads and their dependencies) <code>nvm install node</code>

4. Initialize NPM <code>npm init</code>

5. Install sympm to handle symlinks on VM <code>npm install -g sympm</code> (https://github.com/ezekg/sympm)

6. Initialize sympm <code>sympm install</code>

INCLUDED IN PROVISIONING SCRIPT
When <code>vagrant provision</code> is run, vagrant will install all project dependent software on the VM. If you install any additional development software make sure that it is add to <code>package.json</code> by using the <code>-save--dev</code> flag as in <code>npm install webpack -save--dev</code> If you need to install any software on the VM that is not directly project related, let me know so that I may add it to the provisioning script.


