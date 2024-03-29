Основы JavaScript

# Магические числа

## Вопросы

1. Какой основной принцип именования в программировании?
2. Какой стиль именования используется в JS?
3. Что такое магические числа?
4. Каким должен быть код: коротким или читабельным? Почему?

## Упражнение

`solution.js`

Вы столкнулись с таким кодом, который выводит на экран общее количество комнат во владении нынешнего короля:

```javascript
const king = 'King Balon the 6th';
console.log(king + ' has ' + 6 * 17 + ' rooms.');
```

Как видите, это магические числа: непонятно, что такое 6 и что такое 17. Можно догадаться, если знать историю королевской семьи: каждый новый король получает в наследство все замки от предков и строит новый замок — точную копию родительского. Эта странная династия просто плодит одинаковые замки…

Избавьтесь от магических чисел, создав новые переменные, а затем выведите текст на экран:

```
King Balon the 6th has 102 rooms.
```

Названия переменных должны передавать смысл чисел, но должны при этом оставаться достаточно короткими и ёмкими для комфортного чтения.
