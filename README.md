# Тестовое задание sql

## Описание
В библиотеке размещены книги разных авторов в разных жанрах (стилях). Книги размещены в стеллажах. В каждом стеллаже есть несколько секций, в которых лежат книги, но не более, чем максимальное количество (лимит). У авторов книг, кроме имени, определён период жизни (дата смерти — не обязательный параметр). У каждой книги — стоимость. Библиотека имеет возможность выдавать книги своим подписчикам-абонентам. Так же ведется история выдачи книг этим подписчикам (дата возврата — не обязательный параметр).

Решение должно быть представлено в виде SQL запросов без учёта особенностей отдельных СУБД.

## Структура базы данных

* Авторы — Книги:	1-М
* Стили — Книги:	1-М
* Выдача книг — Книги:	M-M
* Выдача книг – Подписчики:	M-1
* Размещение книг — Книги:	1-1
* Размещение книг — Стеллажи:	1-1

![Структура базы данных](library.png)

## Задания

1. Выдать список названий всех книг в алфавитном порядке, стоимость которых строго меньше 100000
2. Список имён ныне живущих авторов и количество их книг – детективов. (Название в таблице стилей - «Детективы»). Сортировать по количеству книг в порядке по-убыванию.
3. Выдать список самых дорогих книг каждого автора в каждом из жанров.
4. Вывести реестр количества выдачи книг (сколько раз выдавали и количество уникальных книг) по жанрам.
5. Вывести список секций со свободными на текущий момент ячейками.
6. В какой из нормальных форм представлена данная БД?
