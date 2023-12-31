# Строитель (Builder)

**Строитель** — это порождающий паттерн проектирования, который позволяет создавать сложные объекты пошагово. Строитель 
даёт возможность использовать один и тот же код строительства для получения разных представлений объектов.

## Преимущества
🟢 Позволяет создавать продукты пошагово.

🟢 Позволяет использовать один и тот же код для создания различных продуктов.

🟢 Изолирует сложный код сборки продукта от его основной бизнес-логики.

# Недостатки
🔴  Усложняет код программы из-за введения дополнительных классов.
 
🔴 Клиент будет привязан к конкретным классам строителей, так как в интерфейсе директора может не быть метода получения 
результата.

# Цепочка обязанностей (Chain of Responsibility)

**Цепочка обязанностей** — это поведенческий паттерн проектирования, который позволяет передавать запросы последовательно по цепочке обработчиков. Каждый последующий обработчик решает, может ли он обработать запрос сам и стоит ли передавать запрос дальше по цепи.

## Преимущества
🟢 Уменьшает зависимость между клиентом и обработчиками.

🟢 Реализует принцип единственной обязанности.

🟢 Реализует принцип открытости/закрытости.

# Недостатки
🔴 Запрос может остаться никем не обработанным

# Команда (Command)

**Команда** — это поведенческий паттерн проектирования, который превращает запросы в объекты, позволяя передавать их как аргументы при вызове методов, ставить запросы в очередь, логировать их, а также поддерживать отмену операций.

## Преимущества
🟢 Убирает прямую зависимость между объектами, вызывающими операции, и объектами, которые их непосредственно выполняют.

🟢 Позволяет реализовать простую отмену и повтор операций.

🟢 Позволяет реализовать отложенный запуск операций.

🟢 Позволяет собирать сложные команды из простых.

🟢 Реализует принцип открытости/закрытости.

# Недостатки
🔴 Усложняет код программы из-за введения множества дополнительных классов.

# Итератор (Iterator)

**Итератор** — это поведенческий паттерн проектирования, который даёт возможность последовательно обходить элементы составных объектов, не раскрывая их внутреннего представления.

## Преимущества
🟢 Упрощает классы хранения данных.

🟢 Позволяет реализовать различные способы обхода структуры данных.

🟢 Позволяет одновременно перемещаться по структуре данных в разные стороны.

# Недостатки
🔴 Не оправдан, если можно обойтись простым циклом.

# Посредник (Mediator)

**Посредник** — это поведенческий паттерн проектирования, который позволяет уменьшить связанность множества классов между собой, благодаря перемещению этих связей в один класс-посредник.

## Преимущества
🟢 Устраняет зависимости между компонентами, позволяя повторно их использовать.

🟢 Упрощает взаимодействие между компонентами.

🟢 Централизует управление в одном месте.

# Недостатки
🔴 Посредник может сильно раздуться.