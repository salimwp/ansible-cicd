This Ansible playbook is designed to install Git, Jenkins and Apache. Apache is used to offer HTTPS to Jenkins if you want to communicate securely.

The target OS for this Ansible playbook is CentOS 7.7 . To launch this playbook please use the following commands:

```sh
$ mkdir keys
$ ssh-keygen -f keys/myKey
$ python3 -m venv .
$ source bin/activate
$ pip3 install -r requirements.txt
$ ansible-playbook -i hosts -k -K cicd.yaml
```
