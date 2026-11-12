# Учебный Anchor ORM

Небольшая самостоятельно разрабатываемая Java-библиотека для PostgreSQL и
Anchor Modeling в проекте
[bank-learning-project](https://github.com/bank-learning-project).

Библиотека создаётся с нуля по потребностям банковских сценариев.
ORM Finance Lab служит архитектурным образцом для сравнения.

## Целевой объём

- Явные Java-описания anchors, attributes, ties и knots.
- Генерация параметризованных вставок и чтения.
- Собственный Smart Query Builder для запросов по mappings Anchor-модели:
  проекции, фильтры и необходимые связи, SQL с отдельными параметрами и выполнение
  через существующую сессию. Учебные задачи — P2-04 и P2-05.
- Статические и историзируемые атрибуты; текущие и исторические проекции.
- Точные JDBC-преобразования используемых типов.
- Сессия на одном соединении, commit/rollback и освобождение ресурсов.
- Проверки на настоящей PostgreSQL и соответствие mappings миграциям.

Бизнес-правила, ревизии, блокировки агрегатов и миграции принадлежат
[banking](https://github.com/bank-learning-project/banking).
Пул соединений и сборка приложения принадлежат
[app](https://github.com/bank-learning-project/app).
ORM не меняет схему при старте и не открывает JDBC-доступ из UI.

## Документация и обучение

- [Требования](https://github.com/bank-learning-project/app/blob/main/docs/requirements.md)
- [Архитектура](https://github.com/bank-learning-project/app/blob/main/docs/architecture.md)
- [Процесс разработки](https://github.com/bank-learning-project/app/blob/main/docs/development.md)
- [Учебные задачи и зависимости](https://github.com/bank-learning-project/app/blob/main/docs/learning-plan.md)

Сейчас опубликована документация; код и API библиотеки ещё не реализованы.
Разработчик пишет библиотеку самостоятельно небольшими проверяемыми шагами.
Расширения добавляются вместе с использующим их сценарием.
