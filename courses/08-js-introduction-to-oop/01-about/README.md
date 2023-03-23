JS: Введение в ООП

# О курсе

Ключевой частью любого кода являются данные, которые мы получаем, обрабатываем, храним и выводим пользователю. Одни данные устроены просто (строки или массивы), другие сложно (информация о пользователе, включающая десятки и сотни свойств):

```javascript
// В реальности сложнее
const student = {
  name: 'Petya',
  encryptedPassword: ...,
  facebookId: ...,
  payments: [/* платежная информация */],
  currentGroup: ...,
  finishedCourses: [/* список пройденных курсов */]
};
```

Один из способов работы с такими данными - описывать функции, которые их обрабатывают, например меняют пароль. Такой подход называется процедурным программированием:

```javascript
// Внутри себя делает шифрование и обновление user
// user меняется внутри функций
changePassword(user, 'new secret password');
addFinishedCourse(user, finishedCourse);
```

Другой способ - добавить в объекты методы и работать через них:

```javascript
user.changePassword('new secret password');
user.addFinishedCourse(course);
```

**Объектно-ориентированным программированием (ООП)** называется подход, в котором код представляет из себя набор объектов, взаимодействующих друг с другом. Объекты, в таком подходе, это не просто тип данных "объект", это сущности, которые имеют поведение, то есть методы для работы с ними.

## Изучение ООП

Объектно-ориентированное программирование – большая тема, которая пронизывает всю разработку на JavaScript. Ей посвящено сразу несколько курсов, освещающих разные элементы, начиная от синтаксических конструкций, заканчивая подходами в организации кода.

Этот курс знакомит с базовыми концепциями и синтаксисом, немного затрагивает особенности JavaScript, которые сильно выделяют его среди других ООП-языков. Остальные больше посвящены принципам построения программ в ООП стиле и внутренностям самого JS, например, прототипам.

Основные темы:

- Объекты
- Классы
- Инкапсуляция
- Сокрытие данных (Data hiding)
- Исключения

Эти темы важны для начинающего разработчика потому, что с этими понятиями он сталкивается с первых дней на новой работе. Требуется немало времени перед тем, как вы сможете действительно качественно использовать изучаемые подходы и техники. К теме ООП мы вернемся еще не раз: углубим понимание, разберемся с синтаксисом (конструкторами и прототипами).