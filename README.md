# Практический урок: Основы ООП в Python
Добро пожаловать в практический урок по объектно-ориентированному программированию (ООП) в Python! В этом задании вы создадите систему управления персонажами для ролевой игры, используя ключевые концепции ООП.

**Тема**

Создание системы управления персонажами и их инвентаря в фэнтези-игре.
Цели
    *Освоить создание классов, конструкторов и методов.
    *Научиться использовать наследование, инкапсуляцию и другие принципы ООП.
    *Применить практические навыки в написании читаемого и функционального кода.

**Задание**
1. Базовый класс Character

Создайте класс Character, описывающий персонажа в игре.
Требования:

    Конструктор: Определите как минимум 5 атрибутов:
        name (имя, строка)
        health (здоровье, число)
        strength (сила, число)
        gold (золото, число, приватный атрибут)
        weapon (оружие, строка)
    Метод вывода: Реализуйте метод display_info() для красивого вывода информации о персонаже.
    Приватный метод: Добавьте метод __restore_health(), восстанавливающий здоровье до 100, если оно ниже.
    Деструктор: Реализуйте __del__() для вывода сообщения об удалении персонажа.
    Геттер и сеттер: Создайте методы get_gold() и set_gold() для работы с приватным атрибутом gold.

Пример вывода метода display_info():
text
Персонаж: Конан  
Здоровье: 120  
Сила: 20  
Золото: 30  
Оружие: Меч  
2. Создание объектов

Создайте 3 объекта класса Character:

    Воин (например, Конан).
    Маг (например, Мерлин).
    Вор (например, Робин).

3. Удаление объекта

Удалите один из объектов с помощью оператора del и убедитесь, что деструктор сработал.
4. Дочерний класс Merchant

Создайте класс Merchant, наследующийся от Character.
Требования:

    Дополнительные атрибуты:
        inventory (список товаров, например, ["Зелье", "Щит"])
        trade_skill (уровень торговли, число)
    Конструктор: Используйте super() для вызова конструктора родителя и инициализируйте новые атрибуты.
    Переопределение метода: Расширьте display_info() для вывода информации о товарах и навыке торговли.

Пример вывода для Merchant:
text
Персонаж: Альфред  
Здоровье: 80  
Сила: 5  
Золото: 200  
Оружие: Посох  
Товары: ['Зелье', 'Щит', 'Кольцо']  
Навык торговли: 8**
