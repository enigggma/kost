# Лабораторная работа №5

База данных по комплексу гостиниц имеет следующие таблицы:

- Отель: id отеля, название отеля, количество звезд.
- Категория номера: id категории номер, название (люкс, эконом), минимальная площадь по категории.
- Комната отеля: id комнаты, id отеля, id категории номер, номер комнаты в отеле, стоимость суток проживания.
- Клиент: id клиента, фио, телефон.
- Бронирование: id брони, id клиента, дата бронирования
- Комната в бронировании: id комнаты в брони, id брони, id номера, дата заезда, дата выезда.

## Предписание

Номер считается занятым на дату Х,еслидень Х является датой заезда или дата Х находится между датой заезда и выезда.Вдату выезда номер освобождается и доступен для заезда

## Требуется

1. Добавить внешние ключи
2. Выдать информацию о клиентах гостиницы “Космос”, проживающих в номерах категории “Люкс” на 1 апреля 2019г
3. Дать список свободных номеров всех гостиниц на 22 апреля
4. Дать количество проживающих в гостинице “Космос” на 23 марта по каждой категории номеров
5. Дать список последних проживавших клиентов по всем комнатам гостиницы “Космос”, выехавшим в апреле с указанием даты выезда.
6. Продлить на 2 дня дату проживания в гостинице “Космос” всем клиентам комнат категории “Бизнес”, которые заселились 10мая.
7. Найти все "пересекающиеся" варианты проживания. Правильное состояние: не может быть забронированодин номер на одну дату несколько раз, т.к. нельзя заселиться нескольким клиентам в один номер
8. Создать бронирование в транзакции
9. Добавить необходимые индексы для всех таблиц
