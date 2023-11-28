# week15cycles-for-while
Ответы на вопросы по теме:
1. Из скольких частей состоит основной цикл?
Двух - условие и тело

2. Какое количество уровней вложенности могут иметь циклы?
Не ограничено

3. Если switch находится внутри функции, какая инструкция может использоваться для выхода из него?
return

4. Можно ли пропускать части **for**? Что получится, если написать `for(;;)`? 
Да. Будет выполняться бесконечно

5. Самостоятельно разберитесь, как работает цикл while и приведите два примера кода с его использованием.
Цикл while стоит использовать, когда количество итераций заранее неизвестно.
const theNumber = prompt("Введите число от 1 до 5.");  
while (theNumber < 1 || theNumber > 5 || isNaN(theNumber))  
{  
  theNumber = prompt("Введено неправильное значение, пожалуйста, введите число от 1 до 5!");  
}  
alert("Отлично! Вы ввели число: " + theNumber);

6. Как можно принудительно остановить выполнение цикла?
С помощью оператора break, при котором прекращается выполнение текущей итерации цикла.

7. При помощи цикла for выведите чётные числа от 2 до 10.
for (i = 2; i <= 10; i++) {
    if (i % 2 == 0) {
        console.log(i);
    }
}

8. Если тело цикла состоит лишь из одной инструкции, мы можем опустить фигурные скобки `{…}`?
Да

9. Что выведет цикл?
for (let i = 0; i < 3; i++) { 
  console.log(i);
}
Цикл выведет: 0 1 2

10. Оба цикла выводят в консоль одинаковые значения или нет?
let i = 0;
while (++i < 5) console.log(i);

// и

let i = 0;
while (i++ < 5) console.log(i);

В первом случае: 1 2 3 4
Во втором случае: 1 2 3 4 5