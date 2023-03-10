Решение можно проверять онлайн. Для этого достаточно открыть файл solution_issue.ipynb в этом репозитории.

### Локальный запуск нотбука.

#### Требования

Python >= 3.7

#### Инструкция по запуску

1. Скопируйте файлы из этого репозитория в локальную рабочую директорию, перейдите в эту директорию.

2. Создайте виртуальное окружение Python (venv):

```console
$ python3 -m venv <путь к окружению>
```

3. Активируйте окружение

```console
$ . <путь к окружению>/bin/activate
```

4. Установите требуемые пакеты

```console
$ python3 -m pip install -r requirements.txt
```

5. Запустите ноутбук

```console
$ jupyter notebook solution_issue.ipynb
```

#### База данных

Для тестирования использовался ресурс neon.tech, предоставивший базу данных PostgreSQL.

Для загрузки данных в базу данных использовалась следующая команда:

```console
$ psql -d issue_info -h ep-sweet-mode-273478.us-east-2.aws.neon.tech -U guest -c "\copy test from 'data.csv' DELIMITER ';' HEADER csv"
```
Пароль: 0OgVob4ivdXE
