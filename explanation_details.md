## Provision a geerlingguy/ubuntu2004 using vagrant and deploy Yolo app using ansible

## Implementation plan

 ## prerequisites 
  1. install vagrant
  2. Install virtual box.
  3. Install terraform.
  4. Install Ansible.

## Step 1
 Provision a geerlingguy/ubuntu2004 using vagrant using ansible and terraform.

 - create a new branch by the name Stage_two from the main branch.
 - Create a new directory called Stage_two.
 - Change directory to Stage_two
 - create a provider.tf file and add the vagrant provider config.
 - create a variables.tf file to store the variables to be used
 - create a main.tf file where you will add the task for provisioning an ubuntu machine.
 - Run command ` terraform init ` to initialized and load the provider

## Step 2 
Provision an ubuntu virtual machine using ansible and  
Clone and deploy the yolo application in docker desktop.
   ## Deploying the Yolo app
   As has been done in the main branch

  ## Provision the ubuntu virtual machine.
Create a new folder in the roles directory called terraform and then a tasks directory in the created directory.

Create a main.yml file in the roles/terraform/tasks path 

Add the tasks to be executed to deploy the ubuntu machine in main.yml file with includes but not limited to :-
- initialization
- plan
- validate
- apply 

finaly run below command to provision and deploy Yolo app

`
ansible-playbook playbook.yml --tags all
`

Confirm the VM has been deployed and the Yolo app are up and running successfully.