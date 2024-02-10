# A. Не минимум на отрезке

| Параметр            | Условие                          |
|---------------------|----------------------------------|
| Ограничение времени | 1 секунда                        |
| Ограничение памяти  | 64Mb                             |
| Ввод                | стандартный ввод или input.txt   |
| Вывод               | стандартный вывод или output.txt |

Задана последовательность целых чисел a<sub>1</sub>, a<sub>2</sub>, …, a<sub>n</sub>.   
Задаются запросы: сказать любой элемент последовательности на отрезке от **L** до **R** **включительно**, не равный
минимуму
на этом отрезке.

### Формат ввода

В первой строке содержатся два целых числа **N**, 1&nbsp;≤&nbsp;N&nbsp;≤&nbsp;100 и **M**,
1&nbsp;≤&nbsp;M&nbsp;≤&nbsp;1000 — длина последовательности и количество запросов соответственно.

Во второй строке — сама последовательность, 0&nbsp;≤&nbsp;a<sub>i</sub>&nbsp;≤&nbsp;1000.

Начиная с третьей строки перечисляются M запросов, состоящих из границ отрезка L и R,
где L, R - индексы массива, нумеруются с нуля.

### Формат вывода

На каждый запрос выведите в отдельной строке ответ — любой элемент на [L, R], кроме минимального.   
В случае, если такого элемента нет, выведите "NOT FOUND".

### Примеры

##### Пример 1

| **Ввод**                                                              | **Вывод**                                                  |
|-----------------------------------------------------------------------|------------------------------------------------------------|
| 10 5<br/>1 1 1 2 2 2 3 3 3 10<br/>0 1<br/>0 3<br/>3 4<br/>7 9<br/>3 7 | NOT FOUND<br/>2<br/>NOT FOUND<br/>10<br/>3<br/><br/><br/>  |

##### Пример 2

| **Ввод**                         | **Вывод**       |
|----------------------------------|-----------------|
| 10 5<br/>1 1 1 2<br/>0 2<br/>0 3 | NOT FOUND<br/>2<br/><br/><br/> |