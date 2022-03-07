# SQL
SQL queries to different databases

# Databases (полное описание по [ссылке](javascript:openHelp('/help/select13.php#db_1')
  + Компьютерная фирма - 4 таблицы:
    - Product(maker, model, type)
    Таблица Product представляет производителя (maker), номер модели (model) и тип ('PC' - ПК, 'Laptop' - ПК-блокнот или 'Printer' - принтер). Предполагается, что номера моделей в таблице Product уникальны для всех производителей и типов продуктов.
    - PC(code, model, speed, ram, hd, cd, price)
    В таблице PC для каждого ПК, однозначно определяемого уникальным кодом – code, указаны модель – model (внешний ключ к таблице Product), скорость - speed (процессора в мегагерцах), объем памяти - ram (в мегабайтах), размер диска - hd (в гигабайтах), скорость считывающего устройства - cd (например, '4x') и цена - price. 
    - Laptop(code, model, speed, ram, hd, price, screen)
    Таблица Laptop аналогична таблице РС за исключением того, что вместо скорости CD содержит размер экрана -screen (в дюймах).
    - Printer(code, model, color, type, price)
    В таблице Printer для каждой модели принтера указывается, является ли он цветным - color ('y', если цветной), тип принтера - type (лазерный – 'Laser', струйный – 'Jet' или матричный – 'Matrix') и цена - price.
