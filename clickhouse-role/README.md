# Clickhouse Role

Роль для установки и настройки Clickhouse - колоночной СУБД для аналитики.

## Требования

- Ansible 2.9 или выше
- CentOS/RHEL 7 или выше
- Доступ к интернету для загрузки пакетов Clickhouse

## Переменные роли

### Переменные по умолчанию

| Переменная | По умолчанию | Описание |
|------------|--------------|----------|
| clickhouse_version | "22.3.3.44" | Версия Clickhouse для установки |
| clickhouse_packages | ["clickhouse-client", "clickhouse-server", "clickhouse-common-static"] | Список пакетов для установки |
| clickhouse_service_name | clickhouse-server | Имя сервиса Clickhouse |
| clickhouse_database | logs | Имя базы данных для создания |

## Пример использования

```yaml
- hosts: clickhouse
  roles:
    - clickhouse-role
```

## Лицензия

MIT
