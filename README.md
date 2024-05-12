
# Ansible - DevOps Track - NTI
### A brief description of what we did during Ansible Course:

## DAY 1:
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

## DAY 2:
### TAGS
- Write simple playbook file
- Add two tasks (apt update – apt install nginx)
- Add tags to first task: update
- Add tags to second task: install
- Run only the (apt update) task
- Add one task with “tags: always” and run the previous command again
###

## DAY 3:
###
