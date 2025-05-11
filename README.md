# Домашнее задание к занятию 2 «Работа с Playbook»

   ![Task](https://github.com/nick-mp/ansible_Clickhouse_vector_lighthouse/blob/main/img/logo_Vector.png)

   ![Task](https://github.com/nick-mp/ansible_Clickhouse_vector_lighthouse/blob/main/img/logo_ClickHouse.png)

   ![Task](https://github.com/nick-mp/ansible_Clickhouse_vector_lighthouse/blob/main/img/lighthouse.png)   



## Version 

clickhouse_version: "22.3.3.44"

vector_version: "0.39.0"

### Prerequisite

- **Ansible 2.9+**

### Configure

In the file `inventories/host.yml` configure the node details.

### Install

    # Deploy with ansible playbook - run the playbook as root

 
6. Попробуйте запустить playbook на этом окружении с флагом `--check`.

   ![Task](https://github.com/nick-mp/ansible_Clickhouse_vector_lighthouse/blob/main/img/6.png)


7. Запустите playbook на `prod.yml` окружении с флагом `--diff`. Убедитесь, что изменения на системе произведены.

   ![Task](https://github.com/nick-mp/ansible_Clickhouse_vector_lighthouse/blob/main/img/7.png)

8. Повторно запустите playbook с флагом `--diff` и убедитесь, что playbook идемпотентен.

   ![Task](https://github.com/nick-mp/ansible_Clickhouse_vector_lighthouse/blob/main/img/8.png)


есть изменения в таске распаковки lighthouse они из-за того что применяется команда unzip через командную строку.

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.