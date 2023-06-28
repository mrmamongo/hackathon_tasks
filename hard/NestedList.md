Дан список со вложенными списками nestedList. Каждый элемент это либо целое число, либо список. Необходимо реализовать итератор, который будет итерироваться по вложенным спискам включительно

#### Реализация класса NestedIterator:
- NestedIterator(nestedList: List[NestedList]) - конструктор
- next() -> int - возвращает следующий элемент в списке
- hasNext() -> bool - Возвращает True, если может итерироваться дальше, False - если не сможет 

Код будет тестироваться в виде:

```python
class NestedIterator:
    pass

def test():
    nestedList = ...
    iterator = NestedIterator(nestedList)
    res: list[int] = []
    while iterator.hasNext():
        res.append(iterator.next())
    return res
```


### Пример 1:
```
Ввод: nestedList = [[1,1],2,[1,1]]
Вывод: [1,1,2,1,1]
```
### Пример 2:
```
Ввод: nestedList = [1,[4,[6]]]
Вывод: [1,4,6]
```

#### Constraints:
```
1 <= nestedList.length <= 500
The values of the integers in the nested list is in the range [-106, 106].
```

[Ссылочка на задачу](https://leetcode.com/problems/flatten-nested-list-iterator/)