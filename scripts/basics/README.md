# Basic Use Cases
Basic examples of important concepts
## tags.yml
We can run specific tasks by using the name or the task name
- Run a tag
```
ansible-playbook tags.yml -i myhosts --tags ping
```
- You can check tags in a playbook:
```
ansible-playbook tags.yml --list-tags
```
- Run everything except a tag
```
ansible-playbook tags.yml -i myhosts --skip-tags ping
```
- You can also control what is run using task names
```
ansible-playbook tags.yml -i myhosts --start-at-task 'Debug statement'
```
- You can run a playbook **interactively** through tasks
```
ansible-playbook tags.yml -i myhosts --step
```

## localhost.yml
Example of running on localhost
- Run
```
ansible-playbook localhost.yml -i myhosts
```
The ```connection: local``` bypasses ssh which is more resource efficient

## inventory-variables.yml
Use command line and inventory file variables to create a file
- Run
```
ansible-playbook inventory-variables.yml -i myhosts -e file_state=touch 
```