# Role Name

A brief description of the role goes here.

### Who maintains this project
This Ansible Role is maintained by DevIT. If you're looking for help or want to contribute, send an email to any DevIT member.

### Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

### Role Variables

A description of the settable variables for this role should go here, including any variables that are in ``defaults/main.yml``, ``vars/main.yml``, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

```yaml
variable_name: ''

```

### Dependencies

A list of other roles should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

---
### Example Playbook

Import this role `ansible-galaxy install` command, into a roles directory. Reference it through a requirements file to be able to use roles in privately accessible repos. 

*Note: SSH keys setup on local-machine using SSH connection works!* 

[requirements.yml]
```
---
# Importing the ansible xample role
- name: example
  src: "git@github.com:marcmodin/ansible_win_docker.git"
  scm: git
  version: master
```

```yaml
ansible-galaxy install --roles-path ./roles -r requirements.yml
```

A playbook which includes this role could for example look like this
```yaml
- name: Play Name
  hosts: all
  
  vars:
    variable_name: ''
  
  roles:
      - role: role-name
        vars:
          variable_name: ''
```

---

#### Author Information
your name here
