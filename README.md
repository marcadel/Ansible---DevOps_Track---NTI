# Day 2 - Ansible - DevOps Track - NTI
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


