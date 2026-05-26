# Library System

Консольная система управления библиотекой на Python.

## Возможности
- Добавление книг и журналов в библиотеку
- Удаление и поиск по названию, автору, году
- Система аренды: выдача и возврат с датами
- Список просроченных аренд (более 14 дней)
- Сохранение данных между запусками (JSON)
- Покрытие кода юнит-тестами (unittest)

## Структура проекта
```
library_system_pet/
├── library.py        # основная логика
├── models.py         # классы LibraryItem, Book, Magazine
├── tests.py          # юнит-тесты
├── data.json         # база данных
└── README.md
```

## Запуск
```bash
python library.py
```

## Запуск тестов
```bash
python -m unittest tests.py
```

## Классы
- `LibraryItem` — базовый класс
- `Book(LibraryItem)` — книга (жанр, количество страниц)
- `Magazine(LibraryItem)` — журнал (номер выпуска, периодичность)
- `Library` — управление коллекцией и арендой

## Технологии
- Python 3.11
- json
- datetime
- unittest