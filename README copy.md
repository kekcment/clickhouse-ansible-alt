# Clickhouse

Ansible playbook for installation Clickhouse (Altlinux) 

Для установки clickhouse используем следующую команду:
ansible-playbook -i inventory -l clickhouse-cluster clickhouse-playbook.yaml -K

Для указания какие ноды к чему относятся и куда копируется заполнить файл: clusters.xml.j2

Для установки zookeeper используем следующую команду:
ansible-playbook -i inventory -l zookeeper-nodes zookeeper-playbook.yaml -K

Для указания zookeeper нод заполнить файл: zookeeper.xml