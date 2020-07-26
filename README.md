# Ansible-Tower
This is basically devloped for an issue created in https://github.com/ansible/awx/issues/7649 

At first Python script is developed to trigger notification of token expiry in Ansible Tower. 
This python script is executed on localhost from ansible playbook.
Job template is configured in Ansible tower to trigger this ansible playbook and this job scheduled to run daily
This will check no. of tokens getting expired for users in 2 days, 1 day or < 24 hours and notification is sent to repective users based on these conditions
