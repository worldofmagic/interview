# Java Basic Knowledge

## Basic Data Structure -- ArrayList & LinkedList & Vector

ArrayList is implemented as a **resizable array**. As more elements are added to ArrayList, its size is increased dynamically. It's elements can be **accessed directly by using the get and set methods, since ArrayList is essentially an array**. LinkedList is implemented as a **double linked list**. Its performance on **add and remove is better than Arraylist, but worse on get and set methods**. Vector is similar with ArrayList, but it is synchronized. ArrayList is a better choice if your program is thread-safe. Vector and ArrayList require space as more elements are added. Vector each time **doubles** its array size, while ArrayList grow **50%** \(In fact it is 1.5n+1 \) of its size each time. LinkedList, however, also implements Queue interface which adds more methods than ArrayList and Vector, such as offer\(\), peek\(\), poll\(\), etc.

ArrayList has the default capacity of 10 if it is not created with the constructor.

### ArrayList

| get\(\) | O\(1\) |
| :--- | :--- |
| add\(E\) | O\(1\) |
| add\(index, E\)  --------&gt;&gt;&gt;&gt;!!!!! | O\(n\) |
| remove\(\)    --------&gt;&gt;&gt;&gt;!!!!!! | O\(n\) |

The last two functions need to move all the elements forward or backward after the index.

### LinkedList

| get\(\) | O\(n\) |
| :--- | :--- |
| add\(E\) | O\(1\) |
| add\(index, E\)  ----&gt;&gt; need to use get the index first | O\(N\) |
| remove\(\) -----&gt;&gt; actions directly on pointers | O\(1\) |

### 



