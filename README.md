# devops-project
финальный проект по курсу devops

# Запуск
Установить docker и docker-compose, если нет.

Клонировать репозиторий
```bash
git clone https://github.com/Timur1232/devops-project
```

Запустить через docker-compose
```bash
cd devops-project
docker compose up -d
```

# Использование
Открыть Zitadel можно по адресу:
`localhost/zitadel/`

NocoDB по адресу:
`localhost/nocodb/`

Логин и пароль админа zitadel:
- Логин: zitadel-admin@zitadel.localhost
- Пароль: Password1!

Если возникнет проблема с ssl сертификатом, то его можно перегенерировать в директории nginx/certs
```bash
cd nginx/certs
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout localhost.key -out localhost.crt -subj "/CN=localhost"
```
