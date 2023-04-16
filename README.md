# JS_week-13
***** Задание под звездочкой**

Напишите функцию `formatDate(date)`, форматирующую `date` по следующему принципу: 

- если спустя `date` прошло менее 1 секунды, вывести `"прямо сейчас"` ;
- в противном случае, если с `date` прошло меньше 1 минуты, вывести `"n сек. назад"`;
- в противном случае, если меньше часа, вывести `"m мин. назад"`;
- в противном случае, полная дата в формате `"DD.MM.YY HH:mm"`. А именно: `"день.месяц.год часы:минуты"`, всё в виде двух цифр, т.е. `31.12.16 10:00`.
Например:
console.log(formatDate(new Date(new Date - 1))); 
// "прямо сейчас"

console.log(formatDate(new Date(new Date - 30 * 1000))); 
// "30 сек. назад"

console.log(formatDate(new Date(new Date - 5 * 60 * 1000))); 
// "5 мин. назад"

// вчерашняя дата вроде 31.11.2022, 20:00
console.log(formatDate(new Date(new Date - 86400 * 4 * 1000)));
