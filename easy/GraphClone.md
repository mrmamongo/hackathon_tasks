Дана нода в составе замкнутого ненаправленного графа

Вернуть deep copy графа

Каждая нода представлена следующим классом
```python
class Node:
    val: int
    neighbors: list["Node"]
```
 

Формат тестовых кейсов:

Для простоты, значение каждой ноды соответствует индексу ноды (начиная с 1)

Подаваемое на вход значение - список смежных вершин первой ноды - список из unordered list. Каждый из них описывает набор соседей ноды в графе. 

Вводимая нода всегда будет являться нодой с индексом и значением 1. Необходимо вернуть также первую ноду в склонированном графе

 

### Пример 1:
![](https://assets.leetcode.com/uploads/2019/11/04/133_clone_graph_question.png)
```
Ввод: adjList = [[2,4],[1,3],[2,4],[1,3]]
Вывод: [[2,4],[1,3],[2,4],[1,3]]
```
### Пример 2:

```
Ввод: adjList = [[]]
Вывод: [[]]
```
### Пример 3:
```
Ввод: adjList = []
Вывод: []
```

#### Ограничения:
```
0 <= len(graph) <= 100
1 <= Node.val <= 100
Node.val уникальное для каждой ноды
В графах нет повторений.
Любая нода в графе может быть получена из заданной ноды
```

[Ссылочка на задачу](https://leetcode.com/problems/clone-graph/)