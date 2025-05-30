# Vector Role

Роль для установки и настройки Vector - быстрого, легкого и надежного инструмента для сбора, преобразования и отправки логов.

## Требования

- Ansible 2.9 или выше
- CentOS/RHEL 7 или выше
- Доступ к интернету для загрузки пакета Vector

## Переменные роли

### Переменные по умолчанию

| Переменная | По умолчанию | Описание |
|------------|--------------|----------|
| vector_version | "0.39.0" | Версия Vector для установки |
| vector_architecture | "x86_64" | Архитектура системы |
| vector_config_path | /etc/vector/vector.toml | Путь к конфигурационному файлу |
| vector_service_name | vector | Имя сервиса Vector |

## Пример использования

```yaml
- hosts: vector
  roles:
    - vector-role
```

## Лицензия

MIT
