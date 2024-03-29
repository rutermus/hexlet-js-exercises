Основы JavaScript

# Упрощенный синтаксис функций

Определение функции в JS выглядит громоздко:

```javascript
const square = (x) => {
  return x ** 2;
};
```

Здесь используется много дополнительных символов и слово `return`. С версии `es6` в языке появился сокращенный синтаксис, который упрощает восприятие и сокращает количество кода.

```javascript
const double = (x) => x ** 2;
```

Два отличия: пропали фигурные скобки и инструкция `return`. Сокращенная запись функции делает возврат автоматически. Подразумевается, что внутри такой функции одно выражение, которое вычисляется, и его результат возвращается наружу.

Отличия синтаксические и с точки зрения использования различий нет. Пример с двумя аргументами:

```javascript
// Полная версия
const sum = (a, b) => {
  return a + b;
};

// Сокращенная версия
const sum = (a, b) => a + b;
```

Обратите внимание на отсутствие фигурных скобок. Разработчики, которые не привыкли использовать такой синтаксис, иногда пишут подобный код `const sum = (a, b) => { a + b };`, а потом долго не могут понять, почему он не работает. Если стоят фигурные скобки - это не сокращенная форма и для возврата значения нужно поставить `return`.
