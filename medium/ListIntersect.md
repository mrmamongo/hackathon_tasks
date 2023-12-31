Даны головы двух односвязных списков `headA` и `headB`. Вернуть ноду, которая является началом пересечения списков. Если два списка не пересекаются вообще, вернуть `None`

Например, следующие два связных списка начинают пересекаться в ноде `c1`:
![](https://assets.leetcode.com/uploads/2021/03/05/160_statement.png)

Тестовые кейсы гарантируют, что циклов нет ~~хе-хе~~ во всей связной структуре 

#### Внимание

Списки должны сохранить структуру после выполнения кода

### Пример 1:

```
Ввод: intersectVal = 8, listA = [4,1,8,4,5], listB = [5,6,1,8,4,5], skipA = 2, skipB = 3
Вывод: Intersected at '8'
```
### Пример 2:

```
Ввод: intersectVal = 2, listA = [1,9,1,2,4], listB = [3,2,4], skipA = 3, skipB = 1
Вывод: Intersected at '2'
```
### Пример 3:

```
Ввод: intersectVal = 0, listA = [2,6,4], listB = [1,5], skipA = 3, skipB = 2
Вывод: No intersection
 ```

#### Ограничения:

```
len(listA) == m.
len(listB) == n.
1 <= m, n <= 3 * 104
1 <= Node.val <= 105
0 <= skipA < m
0 <= skipB < n
intersectVal == 0 если listA и listB не пересекаются.
intersectVal == listA[skipA] == listB[skipB] если listA и listB пересекаются.
 ```

А чё, сможет кто нибудь: написать решение которое выполняется за O(m + n) времени и использует только O(1) памяти?

[Ссылочка на задачу](https://leetcode.com/problems/intersection-of-two-linked-lists/)