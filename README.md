Simple ansible dnsmasq script.
==============================

Simple script that I use to setup dnsmasq on Centos hosts.
Only breafly tested on Centos 7.


##Example playbook:
### Ansible dnsmasq example playbook
````
---

- hosts: all
  sudo: true
  vars:
    dnsmasq_domain: 'test.org'
    dnsmasq_hosts:
      - name: 'computer2'
        ip: '192.168.1.2'
      - name: 'computer3'
        ip: '192.168.1.3'

  roles:
    - role: ansible-dnsmasq
````

##Author information
Henning Fjellheim
