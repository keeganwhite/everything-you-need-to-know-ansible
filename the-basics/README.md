# The basics of Ansible

## What is ansible
It is a task execution engine that targets local systems and remote systems. Ansible uses a 'clientless' architecture, 
via ssh, so that you do not need to set up and install libraries, packages etc. on the target device. However, we need 
to set up ssh between the host and client machines. The hoist system running ansible is known as the control node.

Ansible is written in Python and Playbooks are written in YAML. 

## Fleet Management
We can manage Ansible in a GUI using Red Hat Ansible Tower (paid) or the open-source equivalent, AWX.

## Advantages of using Ansible
- Ansible is agentless