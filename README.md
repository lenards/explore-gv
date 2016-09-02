# explore-gv

A small example for exploring `group_vars`.


## show the variables for a host

```
ansible -m debug -a "var=hostvars['hostname']" localhost
```
Example: [debug](http://docs.ansible.com/ansible/faq.html#how-do-i-see-all-the-inventory-vars-defined-for-my-host)

http://docs.ansible.com/ansible/setup_module.html

## _dump-all_

I have included a `roles/dump-all` from [CoderWall](https://coderwall.com/p/13lh6w/dump-all-variables).

## playbook debugger / `strategy: debug`

https://docs.ansible.com/ansible/playbooks_debugger.html