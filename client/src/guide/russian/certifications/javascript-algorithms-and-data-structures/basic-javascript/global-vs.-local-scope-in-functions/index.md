---
title: Global vs. Local Scope in Functions
localeTitle: Глобальная и локальная область функций
---
## Глобальная и локальная область функций

Помните, что глобальная область видимости означает, что переменная доступна во всем коде. Локальный масштаб означает, что переменная доступна в определенном диапазоне.

В этом упражнении у вас есть переменная `outerWear` в глобальной области с «футболкой», поскольку это значение. Теперь вы должны создать другую переменную с именем `outerWear` , но на этот раз внутри функции `myOutfit()` . Основное решение для кода:

```javascript
var outerWear = "T-shirt"; 
 
 function myOutfit() { 
  var outerWear = "sweater"; 
  return outerWear; 
 } 
 
 myOutfit(); 
```

Функция вернет ближайший `outerWear` он может найти. Поскольку мы создали `outerWear` функцию внутри функции, то есть «ближайшую», поэтому функция вернет «свитер».