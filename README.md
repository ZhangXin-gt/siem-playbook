# SIEM Playbook Project

## Prerequisite

* python3.8 or newer
* pip3 installed
* poetry installed

## How to start

### Install poetry

```
pip3 install poetry --user -U
```

### Install dependency

```
python -m poetry install
```

### Run playbook


```
cd /path/to/project/root
export ANSIBLE_ROLES_PATH=$PWD/siem/zookeeper/roles:$PWD/siem/kafka/roles

python3 -m poetry run ansible-playbook -i inventory/dev/hosts playbooks/zookeeper.yml
```