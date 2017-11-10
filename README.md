Ansible Workshop 2017
=====================

#### Dutch

Deze repository is gemaakt voor de Ansible workshop 2017, gegeven door Mark, Martin en Jona van [Sentia](https://sentia.com).

De opdracht kan hier worden gevonden: [https://github.com/sentialabs/ansible-workshop/blob/master/ASSIGNMENT.md](https://github.com/sentialabs/ansible-workshop/blob/master/ASSIGNMENT.md).

#### English

This repository is created for the Ansible workshop 2017, given by Mark, Martin and Jona from [Sentia](https://sentia.com).

The assignment can be found here: [https://github.com/sentialabs/ansible-workshop/blob/master/ASSIGNMENT.md](https://github.com/sentialabs/ansible-workshop/blob/master/ASSIGNMENT.md). The assignment is in Dutch.


## Requirements

- Vagrant 1.9.8+
- Internet connection

## Usage with Vagrant

Start the instance. On first boot vagrant will provision the instance using Ansible.

`vagrant up`

## Ansible playbook

The playbook `playbook.yml` will start but is not complete and fail.
It should be completed using the [https://github.com/sentialabs/ansible-workshop/blob/master/ASSIGNMENT.md](https://github.com/sentialabs/ansible-workshop/blob/master/ASSIGNMENT.md).

### Running the playbook

The playbook can be run using either:

#### vagrant provision

This option is less flexible than using ansible-playbook

```
vagrant provision
Provisioning with Ansible started
==> ansible: [vagrant-hostsupdater] Checking for host entries
==> ansible: [vagrant-hostsupdater]   found entry for: 10.0.0.10 ansible
==> ansible: Running provisioner: ansible...
    ansible: Running ansible-playbook...

PLAY [ansible] *****************************************************************

TASK [setup] *******************************************************************
ok: [ansible]

TASK [Install Apache] **********************************************************
ok: [ansible]

```


#### ansible-playbook -i hosts playbook.yml
```
ansible-playbook -i hosts playbook.yml

PLAY [ansible] *****************************************************************

TASK [setup] *******************************************************************
The authenticity of host '[localhost]:2222 ([127.0.0.1]:2222)' can't be established.
ECDSA key fingerprint is SHA256:mVZhzFj5TZ77KLIOxv/KexxoEeO1RyeimVzPlzye2ao.
Are you sure you want to continue connecting (yes/no)? yes
```


License
-------

MIT License

Author Information
------------------
- Mark van der Hout
- Martin Willemsma
- Jona Koudijs
