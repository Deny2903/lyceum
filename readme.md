## Запуск проекта в dev-режиме

### 1. Клонирование репозитория

```bash
git clone https://github.com/Deny2903/lyceum.git
cd lyceum
```

### 2. Создание виртуального окружения
```bash
python3 -m venv .venv
source venv/bin/activate
```

### 3. Установка зависимостей
```bash
pip install -r requirements/dev.txt
```

### 4. Настройка переменных
```bash
cp .env.example .env
```
Вводите свои значения переменных в файле .env

4. Применение миграций
```bash
python manage.py migrate
```

5. Запуск dev-сервера
```bash
python manage.py runserver
```

После запуска проект будет доступен по адресу:
http://127.0.0.1:8000/