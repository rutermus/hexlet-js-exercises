Основы JavaScript

# Интерполяция

Интерполяция - наиболее изящный способ конкатенации строк.

```javascript
const firstName = 'Joffrey';
const greeting = 'Hello';

// Обратите внимание на ограничители строки, это бектики
// Интерполяция не работает с одинарными и двойными кавычками
console.log(`${greeting}, ${firstName}!`);
// => Hello, Joffrey!
```

Мы создали одну строку и «вставили» в нее в нужные места константы с помощью знака доллара и фигурных скобок `${ }`.

Почти во всех языках интерполяция предпочтительнее конкатенации для объединения строк.
