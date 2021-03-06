# Netology-php-diploma

Дипломный проект по программе **"PHP/SQL: back-end разработка и базы данных"** по теме **"Типовой сервис вопросов и ответов (FAQ)".**

## Установка

1. [Установить git](https://git-scm.com/book/ru/v1/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-Git) в нужную директорию, затем клонировать репозиторий:

```
git clone https://github.com/Devyaterikova/diplom.git
```
2. Установить composer
```
composer install
```
3. Скопировать файл конфигурации ```.env.exmaple``` в ```.env```
```
cp  .env.example .env
```
4. Cконфигурировать базу данных, установив необходимые значения полей ```DB_```. **Значение ```DB_DATABASE=faq```.**
5. Сформировать ключ приложения:
```
php artisan key:generate
```
Сформированный ключ будет автоматически добавлен в ```.env```.

6. Восстановить дамп базы данных из файла faq.sql

- Или произвести миграцию базы данных и Заполнить БД  тестовыми данными командами:
```
php artisan migrate
```
```
php artisan db::seed
```

## Панель администрирования

Вход в панель администрирования осуществляется по прямой ссылке **/home**.
При заполнении тестовыми данными в БД создан пользователь с правами администратора:
* Имя: **admin**
* E-mail: **admin@admin.com**
* Пароль: **admin**

## Ссылка на рабочий проект
http://u9118003.beget.tech/index/1

## Описание системы
https://docs.google.com/document/d/1sCpK8XE4g29XUWxjnCPF8WePN5cwa1ZHB9NOCghCfr8/edit?usp=sharing

