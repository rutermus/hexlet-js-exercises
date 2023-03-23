Основы JavaScript

# Неизменяемость и примитивные типы

```javascript
let firstName = 'Alexander';
// Код выполнится без ошибок
firstName[0] = 'B';
console.log(firstName); // => Alexander
// значение переменной firstName останется прежним
```

Причина: неизменяемость примитивных типов в JavaScript — язык не дает возможности поменять строку. Неизменяемость примитивных типов важна по многим причинам, ключевая — производительность. Если нам нужно изменить переменную - перезапишем ее значение:

```javascript
let firstName = 'Alexander';
// Код выполнится без ошибок
firstName = 'Blexander';
console.log(firstName); // => Blexander
```

Есть большая разница между изменением значения переменной и изменением самого значения. Примитивные типы в JavaScript поменять нельзя, а заменить значение переменной можно.

## Слабая типизация

Мы можем складывать числа, т. к. операция сложения — это операция для типа «числа».

Применим эту операцию к числу и строке:

```javascript
console.log(1 + '7'); // => 17
// JS преобразовал число 1 в строку '1',
// и сделал конкатенацию '1' и '7'.
```

Когда JavaScript видит несоответствие типов, он сам пытается преобразовать информацию.

**JavaScript — это язык со слабой типизацией.**

Выполнение любой арифметической операции над строками, кроме сложения, вернет `NaN`:

```javascript
const result = 'one' * 'two';
console.log(result); // => NaN
```

В языках со **строгой типизацией** сложить число со строкой не получится.