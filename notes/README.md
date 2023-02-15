# Ansible Notes

## What is ansible
It is a task execution engine that targets local systems and remote systems. Ansible uses a 'clientless' architecture, 
via ssh, so that you do not need to set up and install libraries, packages etc. on the target device. However, we need 
to set up ssh between the host and client machines. The hoist system running ansible is known as the control node.

Ansible is written in Python and Playbooks are written in YAML.

### Advantages of using Ansible
- Ansible is agentless

### Fleet Management in Ansible
We can manage Ansible in a GUI using Red Hat Ansible Tower (paid) or the open-source equivalent, AWX.

## What are Roles in Ansible
Roles are executable. They can be thought of as a method of automatically loading certain variables, tasks, files, 
templates, and handlers based on a known file structure. Grouping content by roles allows for easy sharing and reuse on
different nodes.

## What are Modules in Ansible
A module is a reusable, standalone script that Ansible runs on your behalf, either locally or remotely. Modules interact
with your local machine, an API, or a remote system to perform specific tasks.

## Ansible for Configuration
Ansible is designed to be minimal in nature. This resulted in it being agentless, SSH-based, state driven and 
idempotent, i.e. all functions can be executed several times without changing the final result beyond its first 
iteration.