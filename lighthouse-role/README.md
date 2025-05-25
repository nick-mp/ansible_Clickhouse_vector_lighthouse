# LightHouse Role

Роль для установки и настройки LightHouse - веб-интерфейса для просмотра логов.

## Требования

- Ansible 2.9 или выше
- CentOS/RHEL 7 или выше
- Доступ к интернету для загрузки LightHouse и установки nginx

## Переменные роли

### Переменные по умолчанию

| Переменная | По умолчанию | Описание |
|------------|--------------|----------|
| lighthouse_nginx_root | /usr/share/nginx/html/lighthouse | Корневая директория для LightHouse |
| lighthouse_nginx_conf_path | /etc/nginx/conf.d/lighthouse.conf | Путь к конфигурационному файлу nginx |
| lighthouse_nginx_service | nginx | Имя сервиса nginx |
| lighthouse_zip_url | https://github.com/VKCOM/lighthouse/archive/refs/heads/master.zip | URL для загрузки LightHouse |
| lighthouse_zip_path | /tmp/lighthouse.zip | Путь для сохранения архива LightHouse |

## Пример использования

```yaml
- hosts: lighthouse
  roles:
    - lighthouse-role
```

## Лицензия

MIT
