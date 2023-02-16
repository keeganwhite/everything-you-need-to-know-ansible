# Basic Use Cases

## tags.yml
We can run specific plays or tasks by using the tag name
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