
# Ansible Update

Ansible para update do SO (Rocky Linux) das máquinas do ambiente virtual via Hyper-V.




## Dependências

```
ansible
ssh-pass
python 3.8 ou superior
```
## Execução do Ansible

Update das máquinas
```bash
  ansible-playbook -i inventory/hosts update.yml -u ${USER} -k -K
```

Limpeza do cache do yum/dnf
```bash
  ansible-playbook -i inventory/hosts clean.yml -u ${USER} -k -K
```
## Etiquetas


[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)

