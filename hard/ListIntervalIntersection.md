Даны два списка с интервалами, где firstList = [starti, endi], secondList = [startj, endj]. Каждый из списков отсортирован и содержит валидные интервалы 

Вернуть пересечение всех интервалов в списках

Закрытый интервал - набор из всех значений x в диапазоне a <= x <= b

Пересечение двух закрытых интервалов - набор целых чисел или пустое множество, которое также является закрытым интервалом. Например, пересечение [1, 3] и [2, 4] это [2, 3]

Пример 1:
![](https://assets.leetcode.com/uploads/2019/01/30/interval1.png)
```
Ввод: firstList = [[0,2],[5,10],[13,23],[24,25]], 
      secondList = [[1,5],[8,12],[15,24],[25,26]]
Вывод: [[1,2],[5,5],[8,10],[15,23],[24,24],[25,25]]
```
Пример 2:
```
Ввод: firstList = [[1,3],[5,9]], secondList = []
Вывод: []
```

Constraints:
```
0 <= firstList.length, secondList.length <= 1000
firstList.length + secondList.length >= 1
0 <= starti < endi <= 109
endi < starti+1
0 <= startj < endj <= 109 
endj < startj+1
```
[Ссылочка на задачу](https://leetcode.com/problems/interval-list-intersections/)