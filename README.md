
# Структура модуля

Библиотека для работы с API amocrm с разделением на подсистемы chats, files и v4. Используется следующая структура
каталогов и файлов.

```
amocrm_api/
│
├── __init__.py                # основной файл пакета, импортирует необходимые модули
│
├── chats/                     # модуль для работы с чатами
│   ├── __init__.py            # инициализация модуля чатов
│   ├── api.py                 # взаимодействие с API чатов (например, получение сообщений)
│   └── utils.py               # вспомогательные функции для работы с чатами (например, парсинг)
│
├── files/                     # модуль для работы с файлами
│   ├── __init__.py            # инициализация модуля файлов
│   ├── api.py                 # взаимодействие с API для загрузки/получения файлов
│   └── utils.py               # вспомогательные функции для работы с файлами
│
├── v4/                        # модуль для работы с API версии 4
│   ├── __init__.py            # инициализация модуля версии 4
│   ├── leads.py               # работа с лидами (например, создание, обновление)
│   ├── contacts.py            # работа с контактами
│   ├── companies.py           # работа с компаниями
│   └── notes.py               # работа с заметками и задачами
│
├── config.py                  # конфигурации для подключения к API (например, токен, URL)
├── auth.py                    # авторизация, работа с токенами и сессиями
└── exceptions.py              # определение ошибок библиотеки
```