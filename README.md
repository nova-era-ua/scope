# Вітаємо в проекті New.Era

## Загальна архитектура

Система будується навколо єдиної бази даних (БД). Всі застосунки звертаються 
до цієї бази. Якшо, в подальшому будуть додаватися якись сервіси (мікросервіси) 
з локальними БД, взаємодія з ними будет вестись шляхом запису/читання з центральної БД.

Від самого початку будем розробляти мультитенантну систему (таку, що дозволяє мати в одній 
фізичній базі даних декілька логічних). Однотенантна система - це окремий випадок 
з фіксованим ідентифікатором тенанту.

Структура БД классична, але є деякі особливості.

Інтерфейс системи побудовано на основі ***розділів***. [Детальніше...](ui.md)


### Елементи системи
* [Ролі в обліку](common/itemrole.md)

Основні сутності системи розподіляются на три великих категорії:

### Довідники

Всі сутності системи поділяються на три чотири великих групи:
* Об'єкти обліку (все, що відповідає на питання "що", "за що"). Всі ці обєкти зберігаются в 
одній таблиці. Назва таблиці - ***Items***.  [Детальніше...](Catalog/items.md)
* Суб'єкти обліку (все, що відповідає на питання "хто" та "куди"). Також зберігаются в 
одній таблиці. Назва таблицы - ***Agents***. [Детальніше...](Catalog/agents.md)
* Інші допоміжні сутності. Такі як одиниці виміру, ставки ПДВ, тощо.

### Документи

### Журнали

## Сруктура інтерфейсу
Користувацький інтерфейс побудовано на основі розділів обліку.

## Додаткова інформація

* [Словник](vocabulary.md)
* [Довідники](Catalog/index.md)
* [Документи](Document/index.md)
* [Журнали](Journal/index.md)

