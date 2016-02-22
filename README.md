# 00

Configurations
===

1. Environment variables list  
---
__STACK_PASSWORD__ : stack user's password( hashed )  
```sh
$ python -c "from passlib.hash import sha512_crypt; print sha512_crypt.encrypt('{{ STACK_PASSWORD }}')"
```
__VBOXNET0_IP__ : IP for ['Host Only Network'](https://www.virtualbox.org/manual/ch06.html#network_hostonly)  
2. `local.conf` 
---
It should be located at `roles/devstack/templates/local.conf`
