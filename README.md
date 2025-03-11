# REST API для игр и жанров
## Используемые инструменты: 
- Язык программирования PHP 8.4
- Пакетный менеджер Composer 2.3.8
- Framework Laravel 12.0.1
- СУБД PostgreSQL
## Основные возможности:
### CRUD операции с жанрами:
- Модель Genre для взаимодействия с сущностью genres
- Класс GenreShowController для показа данных жанров
- Класс GenreCreateController для создания жанров
- Класс GenreChangeController для изменения жанров
- Класс GenreDeleteController для удаления жанров
- Класс GenreController вызывает предыдущие классы. К нему обращается API
### CRUD операции с играми:
- Модель Game для взаимодействия с сущностью games
- Класс GameShowController для показа данных игр
- Класс GameCreateController для создания игр
- Класс GameChangeController для изменения игр
- Класс GameDeleteController для удаления игр
- Класс GameController вызывает предыдущие классы. К нему обращается API
### API
- api.php на полученные запросы get, post, put, delete обращается к классам GenreController и GameController, которые выполняют запрос
