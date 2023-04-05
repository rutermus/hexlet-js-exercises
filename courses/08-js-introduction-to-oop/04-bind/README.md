JS: Введение в ООП

# Связывание (bind)

## Вопросы

1. Для чего нужен метод `bind()`?

   - Он создает новую функцию, связывая исходную функцию с указанным контекстом

2. Что делают функции `call()` и `apply()`?

   - Эти функции внутри себя _меняют контекст_ и _сразу вызывают функцию_. Разница в работе с аргументами функций: `apply()` – принимает аргументы в виде массива вторым параметром, а `call()` ждёт на вход позиционные аргументы.

## Упражнение

`bind.js`

Функции `bind()`, `apply()` и `call()` работают с контекстом и аргументами. В этом упражнении вы научитесь заменять одну функцию другой для получения функциональности, аналогичной `bind()`.

Реализуйте и экспортируйте по умолчанию функцию `bind(obj, fn)`, которая ведет себя аналогично встроенной. Аргументы функции:

- `obj` – объект выступающий в роли контекста
- `fn()` – функция привязываемая к контексту

```javascript
const obj = { number: 5 };
const fn = function fn(number) {
  return number + this.number;
};
const fnWithContext = bind(obj, fn);

// Принимает столько же аргументов сколько и исходная функция

fnWithContext(3); // 8
```

## Примечания

Ограничение: для реализации нельзя пользоваться только встроенной функцией `bind()`.