
# Ansible - DevOps Track - NTI
### A brief description of what we did during Ansible Course:

## DAY 1 - Branch 1:
### INSTALLING ANSIBLE & PREPARING SSH
- Install ansible
- Create a new user on control machine and new user on host 1
- Make sure you can ssh into host 1 (using password)
- Generate SSH key pair on control machine
- Copy the public key to host 1
- Make sure you can ssh into host 1 (using prv/pub)
### INVENTORY FILE
- Create the inventory file
- Put the IP of host 1 in the inventory file
- Use the inventory file path in your ad-hoc command instead of using the IP hard-coded
### CONFIGURATION FILE
- Create the configuration file
- Insert some values in the configuration file
- Run the minimized ad-hoc command
### AD-HOC COMMAND ESCALATION USING ROOT USER
- Insert the correct values in the configuration file
- Example: ansible all -m command -a "whoami"
- What is the output of the command ?
### PLAYBOOK
- Write your first playbook file
- Stop gather_facts and update cache
### MODULES
- Update cache
- Install latest nginx
- Copy index.html from controller to host 1
- Restart nginx service
- Can you see your index.html file when you hit host 1 on port 80 ?

## DAY 2 - Branch 2:
### TAGS
- Write simple playbook file
- Add two tasks (apt update – apt install nginx)
- Add tags to first task: update
- Add tags to second task: install
- Run only the (apt update) task
- Add one task with “tags: always” and run the previous command again
### VARIABLES
Define these variables (package_name, package_version)
- on playbook level
- on inventory level
- on command line level

Use apt module with the package name and version from your variables
### LOOPS
- Loop over a list of packages and install latest versions.
- Loop over a list of packages and use different states as per input.
### WHEN
- Install nginx or httpd depending on distribution
- Restart nginx service if distribution is ubuntu.
- Restart httpd service if distribution is centos.
### REGISTER
- View the value of your register variable using debug module
- Restart service if the installation task was changed or was not failed
### HANDLERS
- install a package (get the package name from vars)
- copy a list of files (index.html & file.css & file.js) from controller to host using loop
- Restart the service of the installed package
### TEMPLATES
- installing a package
- Copying index.html from controller to host using template
- copying a list of files (file.css & file.js) from controller to host using loop
- Restart the service of the installed package





## DAY 3 - Branch 3:
### ROLES
- Create your first role with name (web)
- #### The task book will include:
- installing a package
- Copying a file from controller to host using template
- copying a list of files from controller to host using loop
- Restart the service of the installed package

