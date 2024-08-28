# Datetime_RUS_EDITION

The datetime module supplies classes for manipulating dates and times.// Python

REFERENCES: https://stepik.org/course/82541 - "Поколение Python": курс для профессионалов

# 1. Модуль date и time

Используется для:

1. Получения текущих даты и времени.
2. Сравнение даты или времени
3. Проведения арифметических действия над датой или временем
4. Получения форматированного ввода данных о дате или времени.

Существует две формы представления даты и времени: формальные ( понимает компьютер ) и неформальные ( понимает человек ) строковые представления. Методы str() and repr() помогают такие представления.

Если данные помещены в список , то представление будет формальным . Чтобы получить неформальное представление , то нужно список распаковать.

Тип date и time являются неизменяемыми.

По умолчанию объекты типов date и time выводятся в ISO 8601 формате:

В качестве ограничений по годам в типе date используются значения MINYEAR=1 и MAXYEAR=9999

# Тип date:

Атрибуты
1. .year,.month,.day
2. .min, .max - 0001-01-01, 9999-12-31 - минимальные и максимально возможные даты
Методы
1. .today()
2. .weekday() . Дни недели от 0 до 6 дней
3. .isowedkday(). Дни недели от 1 до 7
4. date.fromordinal(numbers of days ) - получение даты по числу дней начиная от минимальной даты - метод класса date
5. date1.toordinal() - перевод даты в дни начиная от минимальной - метод экземпляра date

# Тип time:

Атрибуты:
1. hour , minute, second, microsecond

Как-то мало совсем о времени. Надо глянуть

С данными типами можно пользоваться функциями min(), max(), sorted()

Также существует полезный метод .replace() , который позволяет заменять старые данные о дате и времени на новые.
