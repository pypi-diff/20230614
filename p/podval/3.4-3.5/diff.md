# Comparing `tmp/podval-3.4.tar.gz` & `tmp/podval-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-3.4.tar", last modified: Wed Jun 14 10:37:19 2023, max compression
+gzip compressed data, was "dist\podval-3.5.tar", last modified: Wed Jun 14 19:36:42 2023, max compression
```

## Comparing `podval-3.4.tar` & `podval-3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 10:37:19.000000 podval-3.4/
--rw-rw-rw-   0        0        0      188 2023-06-14 10:37:19.000000 podval-3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 10:37:19.000000 podval-3.4/podval/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.4/podval/__init__.py
--rw-rw-rw-   0        0        0    50824 2023-06-14 10:26:28.000000 podval-3.4/podval/exam.py
--rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.4/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.4/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 10:37:19.000000 podval-3.4/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 10:37:19.000000 podval-3.4/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-14 10:33:14.000000 podval-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:36:42.000000 podval-3.5/
+-rw-rw-rw-   0        0        0      188 2023-06-14 19:36:42.000000 podval-3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 19:36:42.000000 podval-3.5/podval/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.5/podval/__init__.py
+-rw-rw-rw-   0        0        0    86591 2023-06-14 19:36:17.000000 podval-3.5/podval/exam.py
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.5/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.5/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 19:36:42.000000 podval-3.5/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-14 19:36:28.000000 podval-3.5/setup.py
```

### Comparing `podval-3.4/podval/exam.py` & `podval-3.5/podval/exam.py`

 * *Files 20% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
 print("Изначальный список:", dllist)
 max_value = find_and_remove_max(dllist)
 print("Максимальное значение:", max_value)
 print("Список после удаления максимального элемента:", dllist)''')
 
 #2    
-def lpschs():
+def lpschsi():
     print('''#Отфильтровать список целых чисел на простые и составные числа с помощью лямбда-функции.
 
 # Заданный список целых чисел
 numbers = [2, 3, 4, 5, 6, 7, 8, 9, 10]
 
 # Лямбда-функция для проверки числа на простоту
 is_prime = lambda num: all(num % i != 0 for i in range(2, int(num**0.5) + 1)) and num > 1
@@ -839,14 +839,767 @@
 for item in items:
     tree.insert(item)
 
 # вывод бинарного дерева на экран
 print(items)
 print(tree)
 tree.height()''')
+
+#6   
+def pyaksz():
+    print('''#Используя лямбда-функцию, найдите все числа в заданном списке,
+которые являются палиндромами.
+my_list = [121, 55, 4664, 10, 12321, 88, 67876]
+palindromes = filter(lambda x: str(x) == str(x)[::-1], my_list)
+print(list(palindromes))''')
+  
+def skvbg():
+    print('''#Напишите программу для сортировки заданного списка строк по
+количеству гласных букв в каждой строке
+my_list = ['apple', 'peach', 'banana', 'watermelon', 'aboooooooooooba', 'lol', 'kk']
+
+def count_vowels(word):
+  vowels = 'aeiouAEIOU'
+  k = 0
+  for letter in word:
+    if letter in vowels:
+      k += 1
+  return k
+
+
+sorted_list = sorted(my_list, key = count_vowels)
+print(sorted_list)''')
+    
+def chsrchd():
+    print('''#Используя лямбда-функцию, найдите все числа в заданном списке,
+которые являются совершенными числами (сумма делителей числа
+равна самому числу).
+my_list = [6, 12, 28, 9, 496, 99, 8128, 24]
+perfect_nums = filter(lambda x: sum([i for i in range(1, x) if x % i == 0]) == x, my_list)
+print(list(perfect_nums))''')
+
+def pdbvz():
+    print('''#Найти наибольший элемент, меньший заданного значения, в бинарном дереве поиска.
+class Node:
+    def __init__(self, data):
+        self.data = data
+        self.left = None
+        self.right = None        
+
+class BinaryTree:
+    def __init__(self):
+        self.root = None
+
+    def insert(self, data):
+        new_node = Node(data)
+        if self.root is None:
+            self.root = new_node
+        else:
+            current = self.root
+            while True:
+                if data < current.data:
+                    if current.left is None:
+                        current.left = new_node
+                        break
+                    else:
+                        current = current.left
+                else:
+                    if current.right is None:
+                        current.right = new_node
+                        break
+                    else:
+                        current = current.right
+
+    def search(self, data):
+        current = self.root
+        while current is not None:
+            if data == current.data:
+                return True
+            elif data < current.data:
+                current = current.left
+            else:
+                current = current.right
+        return False
+
+    def delete(self, data):
+        if self.root is not None:
+            self.root = self._delete(data, self.root)
+
+    def _delete(self, data, node):
+        if node is None:
+            return node
+
+        if data < node.data:
+            node.left = self._delete(data, node.left)
+        elif data > node.data:
+            node.right = self._delete(data, node.right)
+        else:
+            if node.left is None:
+                return node.right
+            elif node.right is None:
+                return node.left
+
+            temp = self._find_min_node(node.right)
+            node.data = temp.data
+            node.right = self._delete(temp.data, node.right)
+
+        return node
+
+    def _find_min_node(self, node):
+        while node.left is not None:
+            node = node.left
+        return node
+
+    def __str__(self):
+        return '\n'.join(self._display(self.root)[0])
+
+    def _display(self, node):
+        if node.right is None and node.left is None:
+            line = str(node.data)
+            width = len(line)
+            height = 1
+            middle = width // 2
+            return [line], width, height, middle
+
+        if node.right is None:
+            lines, n, p, x = self._display(node.left)
+            s = str(node.data)
+            u = len(s)
+            first_line = (x + 1)*' ' + (n - x - 1)*'_' + s
+            second_line = x*' ' + '/' + (n - x - 1 + u)*' '
+            shifted_lines = [line + u*' ' for line in lines]
+            return [first_line, second_line] + shifted_lines, n + u, p + 2, n + u // 2
+
+        if node.left is None:
+            lines, n, p, x = self._display(node.right)
+            s = str(node.data)
+            u = len(s)
+            first_line = s + x*'_' + (n - x)*' '
+            second_line = (u + x)*' ' + '\\' + (n - x - 1)*' '
+            shifted_lines = [u*' ' + line for line in lines]
+            return [first_line, second_line] + shifted_lines, n + u, p + 2, u // 2
+
+        left, n, p, x = self._display(node.left)
+        right, m, q, y = self._display(node.right)
+        s = str(node.data)
+        u = len(s)
+        first_line = (x + 1)*' ' + (n - x - 1)*'_' + s + y*'_' + (m - y)*' '
+        second_line = x*' ' + '/' + (n - x - 1 + u + y)*' ' + '\\' + (m - y - 1)*' '
+        if p < q:
+            left += [n*' ']*(q - p)
+        elif q < p:
+            right += [m*' ']*(p - q)
+        zipped_lines = zip(left, right)
+        lines = [first_line, second_line] + [a + u*' ' + b for a, b in zipped_lines]
+        return lines, n + m + u, max(p, q) + 2, n + u // 2
+
+
+
+def find_max(node, x):
+  values = []
+  if node == None:
+    return []
+  elif node.data < x:
+    values.append(node.data)
+  values += find_max(node.left, x)
+  values += find_max(node.right, x)
+  return values
+
+
+from random import shuffle
+t = list(range(1, 11))
+shuffle(t)
+tree = BinaryTree()
+for i in t:
+  tree.insert(i)
+
+print(tree)
+
+
+a = max(find_max(tree.root, 9))
+a''')
+    
+#7
+def tstsirr():
+    print('''#Создайте класс «Круг» с атрибутами радиус и цвет. Напишите методы
+для вычисления площади и длины окружности круга. Используйте
+магический метод __str__ для вывода информации о круге в виде «Круг
+радиуса {радиус} и цвета {цвет}»
+from math import pi
+
+class Circle():
+
+  def __init__(self, radius, color = 'transparent'):
+    self.radius = radius
+    self.color = color
+
+  def area(self):
+    return pi * self.radius ** 2
+
+  def length(self):
+    return 2 * pi * self.radius
+
+  def __str__(self):
+    return f'Круг радиуса {self.radius} и цвета {self.color}'
+    
+c = Circle(3, 'red')
+print(c)''')
+    
+    
+def sdvem():
+    print('''#Реализовать функцию, которая находит минимальный элемент в двусвязном списке
+
+class Node():
+
+  def __init__(self, data = None):
+    self.data = data
+    self.next = None
+    self.prev = None
+
+class DoublyLinkedList():
+
+  def __init__(self):
+    self.head = None
+
+  def add_node(self, data):
+    new_node = Node(data)
+
+    if self.head is None:
+      self.head = new_node
+    else:
+      cur = self.head
+      while cur.next:
+        cur = cur.next
+      cur.next = new_node
+      new_node.prev = cur
+  
+  def find_min(self):
+    if self.head == None:
+      return 'the list is empty'
+
+    cur = self.head
+    min = float('inf')
+    while cur.next:
+      if cur.data < min:
+        min = cur.data
+      cur = cur.next
+    if cur.data < min:
+      min = cur.data
+
+
+    return min
+
+  
+  def __str__(self):
+    if self.head == None:
+      return 'the list is empty'
+    else:
+      st = ''
+      cur = self.head
+      while cur:
+       st += str(cur.data) + ' <-> '
+       cur = cur.next
+      return st.strip(' <-> ')
+
+nums = [10, 9, 8, 4, 3, 9, 4, 0]
+n =  DoublyLinkedList()
+for i in nums:
+  n.add_node(i)
+
+print(n)
+print(n.find_min())''')
+    
+#8    
+def vvisv():
+    print('''#Создайте класс «Студент» с атрибутами имя, возраст и список оценок.
+Напишите методы для вычисления среднего балла и определения
+успеваемости студента (средний балл выше 4). Используйте магический
+метод __repr__ для вывода информации о студенте в виде «Студент
+{имя}, возраст {возраст}»
+class Student():
+  def __init__(self, name, age, marks = None):
+    self.name = name
+    self.age = age
+    self.marks = marks if marks is not None else []
+  
+  def average_score(self):
+    if self.marks is not None:
+      return sum(self.marks)/len(self.marks)
+    else:
+      return 'no marks'
+
+  def performance(self):
+    if self.average_score() > 4.0:
+      return 'good student'
+    else:
+      return 'bad student'
+
+  def __repr__(self):
+    return f'Студент {self.name}, возраст {self.age}'
+''')
+
+
+def ddnot():
+    print('''#Создать класс очереди, который будет хранить только элементы,
+большие заданного значения. Значение задается при инициализации
+объекта класса очереди. При добавлении элемента, если он меньше или
+равен заданному значению, то он не должен добавляться.
+class Node:
+    def __init__(self, data):
+        self.data = data
+        self.next = None
+
+class Queue():
+    def __init__(self, limit = 0):
+        self.head = None
+        self.tail = None
+        self.limit = limit
+
+    def is_empty(self):
+        return not bool(self.head)
+
+    def enqueue(self, data):
+        if data > self.limit:
+            new_node = Node(data)
+            if not self.head:
+                self.head = new_node
+                self.tail = new_node
+            else:
+                self.tail.next = new_node
+                self.tail = new_node
+
+    def dequeue(self):
+        data = self.head.data
+        self.head = self.head.next
+        if not self.head:
+            self.tail = None
+        return data
+
+    def __len__(self):
+        count = 0
+        current = self.head
+        while current:
+            count += 1
+            current = current.next
+        return count
+
+    def __str__(self):
+        current = self.head
+        queue_str = ""
+        while current:
+            queue_str += " → " + str(current.data)
+            current = current.next
+        return queue_str.lstrip(" → ")  
+
+
+q1 = Queue(5)
+nums = [1, 2, 3, 4, 5, 6, 7, 8, 9]
+for i in range(len(nums)):
+  q1.enqueue(i)
+print(q1)''')
+    
+#9    
+def pavzs():
+    print('''#Используя лямбда-функцию, отсортировать список строковых значений в алфавитном порядке.
+fruits = ['apple', 'Orage', 'peach', 'kiwi', 'Banana', 'grapes', 'Lemon']
+sorted(fruits, key=lambda x: x[0].lower())''')
+    
+    
+def lpsss():
+    print('''#Найдите все анаграммы в заданном списке строк с помощью лямбда-функции
+words = ['нос','апельсин', 'собака', 'тапок', 'топка',  'автор', 'шакал',  'отвар', 'товар', 'алкаш', 'шкала', 'кот', 'капот', 'покат', 'ток', 'сон', 'кошка']
+anagrams_dict = {}
+for w in words:
+  key = ''.join(sorted(w))
+  anagrams_dict[key] = []
+  for ww in words:
+    if key == ''.join(sorted(ww)):
+      anagrams_dict[key].append(ww)
+
+result = list(filter(lambda x: len(x) > 1, anagrams_dict.values()))''')
+    
+    
+def lpschsz():
+    print('''#Найти индекс и значение максимального и минимального значений в заданном списке чисел с помощью лямбда-функции.
+nums = [876, 9, 3, 4, 5, 6, 876, 453, 98, 543, 48] 
+max_index, max_value = max(enumerate(nums), key=lambda x: x[1])
+min_index, min_value = min(enumerate(nums), key=lambda x: x[1])
+
+print("Максимальное значение:", max_value)
+print("Индекс максимального значения:", max_index)
+print("Минимальное значение:", min_value)
+print("Индекс минимального значения:", min_index)''')
+    
+    
+def sepdya():
+    print('''#Дан стек. Необходимо удалить из него все элементы, которые не являются делителями последнего элемента стека.
+class Node:
+    def __init__(self, data):
+        self.data = data
+        self.next = None
+
+class Stack:
+    def __init__(self):
+        self.head = None
+
+    def is_empty(self):
+        return self.head is None
+
+    def push(self, item):
+        new_node = Node(item)
+        new_node.next = self.head
+        self.head = new_node
+
+    def pop(self):
+        if self.is_empty():
+            return None
+        else:
+            popped_item = self.head.data
+            self.head = self.head.next
+            return popped_item
+
+    def peek(self):
+        if self.is_empty():
+            return None
+        else:
+            return self.head.data
+    
+
+    def __str__(self):
+        current = self.head
+        stack_str = ""
+        while current:
+            stack_str += str(current.data) + " → "
+            current = current.next
+        return stack_str.rstrip(" → ")
+
+
+def remove_non_divisors(stack):
+    last_element = stack.pop()
+    
+    print(last_element)
+    new_stack = Stack()
+    new_stack.push(last_element)
+    cur = stack.head
+    while cur:
+        if  last_element % cur.data == 0:
+            new_stack.push(cur.data)
+        cur = cur.next
+    
+    return new_stack
+
+
+
+stack = Stack()
+
+# добавление элементов в стек
+from random import randint
+
+for i in range(10):
+    stack.push(randint(1, 10))
+
+# вывод стека на экран
+print(f'Стек: {stack}')
+
+stack = remove_non_divisors(stack)
+print(f'Стек: {stack}')''')
+
+#10
+def evpks():
+    print('''#Используя лямбда-функцию, отсортировать список кортежей по второму элементу.
+my_list = [(3, 4), (1, 2), (5, 7), (2, 8)]
+sorted_list = sorted(my_list, key=lambda x: x[1])
+print(sorted_list)''')
+    
+def lichsz():
+    print('''#Найти все числа, которые делятся на три или пять, из заданного списка чисел, используя лямбда-функцию.
+my_list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+three_five = list(filter(lambda x: x % 3 == 0 or x % 5 == 0, my_list))
+three_five''')
+    
+    
+def chpobd():
+    print('''#Напишите программу для сортировки заданного смешанного списка
+#целых чисел и строк с помощью лямбда-функции. Строки должны быть
+#отсортированы перед числами
+lst=[1,2,"bb",3,0,"aa","%%"]
+print(sorted(list(filter(lambda x: type(x) is str,lst))) + sorted(list(filter(lambda x: type(x) is not str,lst))))
+''')
+    
+    
+def nneei():
+    print('''#Написать функцию, которая принимает на вход двусвязный список
+#и значение элемента, который нужно найти. Функция должна вернуть
+#индекс первого вхождения элемента в список или -1, если элемент не
+#найден.
+
+class Node:
+    def __init__(self, data):
+        self.data = data
+        self.prev = None
+        self.next = None
+
+class DoublyLinkedList:
+    def __init__(self):
+        self.head = None
+
+    def add_node(self, data):
+        new_node = Node(data)
+        if self.head is None:
+            self.head = new_node
+        else:
+            current = self.head
+            while current.next is not None:
+                current = current.next
+            current.next = new_node
+            new_node.prev = current
+
+    def delete_node(self, data):
+        if self.head is None:
+            return
+        elif self.head.data == data:
+            if self.head.next is not None:
+                self.head = self.head.next
+                self.head.prev = None
+            else:
+                self.head = None
+        else:
+            current = self.head
+            while current.next is not None and current.next.data != data:
+                current = current.next
+            if current.next is None:
+                return
+            else:
+                current.next = current.next.next
+                if current.next is not None:
+                    current.next.prev = current
+
+    def __len__(self):
+        count = 0
+        current = self.head
+        while current:
+            count += 1
+            current = current.next
+        return count
+
+    def __str__(self):
+        if self.head == None:
+            return f"Двусвязный список пустой"
+        current = self.head
+        dllist_str = ""
+        while current:
+            dllist_str += " ⇄ " + str(current.data)
+            current = current.next
+        return dllist_str.lstrip(" ⇄ ") 
+
+def find_ind(dllist, x):
+    current_node = dllist.head
+    c = 0
+    while current_node:
+        if current_node.data == x:
+          return c
+
+        c += 1   
+        current_node = current_node.next
+    return -1
+        
+dll = DoublyLinkedList()
+from random import randint
+
+# добавление элементов в двухсвязный список
+for i in range(randint(5,10)):
+    dll.add_node(randint(1,20))
+
+# вывод двусвязного списка на экран
+print(f'Двусвязный список (len = {len(dll)}): {dll}')
+print(find_ind(dll, 1))''')
+
+#11
+def nipchd():
+    print('''# С помощью лямбда-функции проверьте, является ли данное число простым или нет
+is_prime = lambda num: all(num % i != 0 for i in range(2, int(num ** 0.5) + 1)) and num > 1
+print(is_prime(7))   # Output: True
+print(is_prime(20))  # Output: False''')
+    
+    
+def dodzp():
+    print('''#Напишите программу для поиска чисел в заданном диапазоне, которые являются суммой двух квадратов. Пример: задан диапазон от 1
+#до 50 → [1, 2, 4, 5, 8, 9, 10, 13, 16, 17, 18, 20, 25, 26, 29, 32, 34, 36, 37, 40,
+#41, 45, 49, 50]
+def sumSquare(n):
+ 
+    s = dict()
+    for i in range(1, n):
+ 
+        if i * i > n:
+            break
+ 
+        # store square value in hashmap
+        s[i * i] = 1
+ 
+        if (n - i * i) in s.keys():
+            print((n - i * i)**(1 / 2),
+                       "^2 +", i, "^2")
+            return True
+         
+    return False
+
+lst = [1, 2, 4, 5, 8, 9, 10, 13, 16, 17, 18, 20, 25, 26, 29, 32, 34, 36, 37, 40, 41, 45, 49, 50]
+ss = list(filter(lambda x: (sumSquare(x)), lst))
+ss''')
+    
+    
+def psdvp():
+    print('''#Удалите все элементы из заданного списка, не присутствующие в другом списке. Пример: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], [2, 4, 6, 8] → [2, 4, 6, 8]
+lst1 = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+lst2 = [2, 4, 6, 8, 13, 25]
+lst1 = [i for i in lst1 if i in lst2]
+
+print(lst1)''')
+    
+    
+def tyaovkh():
+    print('''#Создать класс хеш-таблицы для хранения объектов класса «Сотрудник».
+#Хеш-функция должна основываться на поле «должность» сотрудника.
+#Если два сотрудника имеют одну и ту же должность, они должны
+#храниться в одной ячейке таблицы
+
+class HashTable:
+    def __init__(self, size):
+        self.size = size
+        self.table = [[] for _ in range(self.size)]
+
+    def hash_function(self, key):
+        return hash(key) % self.size
+
+    def insert(self, Employee):
+        index = self.hash_function(Employee.position)
+        self.table[index].append(Employee.name)
+
+    def find(self, position):
+        index = self.hash_function(position)
+        return self.table[index]
+        
+class Employee:
+    def __init__(self, position, name):
+        self.position = position
+        self.name = name
+
+    def __str__(self):
+        return f"Должность: {self.position}, имя: {self.name}"
+        
+Employees = HashTable(6)
+employees_list = [Employee('Programmer', 'Boris Godunov'), Employee('Programmer', 'Ilya'),
+              Employee('Manager', 'Anna')]
+for b in employees_list:
+    Employees.insert(b)
+    print(b)
+
+print(Employees.find('Programmer'))
+''')
+
+#12    
+def dtiyai():
+    print('''#Опишите класс Recipe, заданный названием, списком ингредиентов
+#и шагами приготовления. Включите в описание класса методы: вывода
+#информации о рецепте на экран, проверки, есть ли все ингредиенты для
+#приготовления блюда, и свойство, позволяющее установить тип кухни
+#(например, итальянская, японская и т. д.).
+class Recipe:
+    def __init__(self, name, ingredients, steps):
+        self.name = name
+        self.ingredients = ingredients
+        self.steps = steps
+        self._cuisine_type = ""
+
+    def display_recipe(self):
+        print(f"{self.name}\nIngredients: {self.ingredients}\nSteps:")
+        for i, step in enumerate(self.steps, start=1):
+            print(f"{i}. {step}")
+
+    def check_ingredients(self, available_ingredients):
+        for ingredient in self.ingredients:
+            if ingredient not in available_ingredients:
+                return False
+        return True
+
+    @property
+    def cuisine_type(self):
+        return self._cuisine_type
+
+    @cuisine_type.setter
+    def cuisine_type(self, cuisine):
+        self._cuisine_type = cuisine
+
+recipe = Recipe("Pasta with tomato sauce", ["pasta", "tomatoes", "garlic"], ["Cook pasta", "Make tomato sauce", "Combine pasta and sauce"])
+
+recipe.display_recipe()
+
+if recipe.check_ingredients(["pasta", "tomatoes", "garlic"]):
+    print("I have all the ingredients")
+else:
+    print("I need to buy some ingredients")
+
+recipe.cuisine_type = "Italian"
+print(recipe.cuisine_type)''')
+
+    
+def siidm():
+    print('''#Написать метод класса «Заказ», который сортирует список заказов по
+#дате с помощью алгоритма быстрой сортировки. Метод должен
+#изменять исходный список.
+
+
+class Order:
+    def __init__(self, id, date, amount):
+        self.id = id
+        self.date = date
+        self.amount = amount
+        
+class OrderList:
+    def __init__(self, orders):
+        self.orders = orders
+        
+    def sort_by_date(self):
+        self._quicksort(0, len(self.orders) - 1)
+        
+    def _quicksort(self, start, end):
+        if start >= end:
+            return
+        
+        pivot_idx = self._partition(start, end)
+        self._quicksort(start, pivot_idx - 1)
+        self._quicksort(pivot_idx + 1, end)
+        
+    def _partition(self, start, end):
+        pivot = self.orders[end].date
+        i = start - 1
+        
+        for j in range(start, end):
+            if self.orders[j].date <= pivot:
+                i += 1
+                self.orders[i], self.orders[j] = self.orders[j], self.orders[i]
+                
+        self.orders[i + 1], self.orders[end] = self.orders[end], self.orders[i + 1]
+        return i + 1
+
+
+
+orders = [
+    Order(1, "2021-01-01", 100),
+    Order(2, "2021-02-01", 200),
+    Order(3, "2021-01-15", 150),
+    Order(4, "2021-03-01", 75),
+]
+
+order_list = OrderList(orders)
+order_list.sort_by_date()
+
+for order in order_list.orders:
+    print(order.date)''')
     
 #13
 def chpyaks():
     print('''# а) Используя лямбда-функцию, найдите все числа в заданном списке, которые являются простыми числами.
 import numpy as np
 lst = np.random.randint(1, 100, 30)
 A = list(filter(lambda a: np.sum([i for i in range (2, a) if a % i == 0]) == 0, lst))
@@ -1459,8 +2212,368 @@
 
 q.enqueue(0.6)
 print(q)
 
 q.enqueue(6)
 print(q)
 
-print(q.get_queue())''')
+print(q.get_queue())''')
+    
+#19_____________________________________________
+
+#20
+def kchyaks():
+    print('''Используя лямбда-функцию, найдите все числа в заданном списке, которые являются числами Капрекара.
+lst = [9, 12, 43, 15, 45, 55, 99, 297, 703, 999]
+a = list(filter(lambda x : x in [int(str(x**2)[:i]) + int(str(x**2)[i:]) for i in range(1, len(str(x**2))) if int(str(x**2)[i:]) != 0 and int(str(x**2)[:i]) + int(str(x**2)[i:])], lst))
+a''')
+
+def applv():
+    print('''Напишите программу для сортировки заданного списка строк в лексикографическом порядке (по алфавиту).
+a = ['aa', 'ab', 'aaabbb', 'abc', 'aabbcc', 'aab']
+b = ['корова', 'корона', 'король', 'коррида', 'корвалол']
+
+def insertion_sort(arr):
+    for i in range(1, len(arr)):
+        key = arr[i]
+        j = i - 1
+        while j >= 0 and arr[j] > key:
+            arr[j + 1] = arr[j]
+            j -= 1
+        arr[j + 1] = key
+    return arr
+
+insertion_sort(a)
+
+insertion_sort(b)''')
+
+def achyaks():
+    print('''Используя лямбда-функцию, найдите все числа в заданном списке, которые являются числами Армстронга.
+b = [12, 153, 407, 370, 371, 432]
+k = list(filter(lambda x: x == sum([i**len(list(map(int, str(x)))) for i in list(map(int, str(x)))]) , b))
+print(k)''')
+
+def sdvek():
+    print('''#Реализовать функцию, которая находит количество элементов в двусвязном списке.
+class Node:
+    def __init__(self, data):
+        self.data = data
+        self.prev = None
+        self.next = None
+
+class DoublyLinkedList:
+    def __init__(self):
+        self.head = None
+
+    def add_node(self, data):
+        new_node = Node(data)
+        if self.head is None:
+            self.head = new_node
+        else:
+            current = self.head
+            while current.next is not None:
+                current = current.next
+            current.next = new_node
+            new_node.prev = current       
+
+    def __len__(self):
+        count = 0
+        current = self.head
+        while current:
+            count += 1
+            current = current.next
+        return count
+
+    def __str__(self):
+        if self.head == None:
+            return f"Двусвязный список пустой"
+        current = self.head
+        dllist_str = ""
+        while current:
+            dllist_str += " ⇄ " + str(current.data)
+            current = current.next
+        return dllist_str.lstrip(" ⇄ ")
+
+import numpy as np
+x = DoublyLinkedList()
+for i in range(12):
+    x.add_node(np.random.randint(0, 1000, 1)[0])
+
+print(x)
+
+print(len(x))''')
+
+#21
+def suknf():
+    print('''#Опишите класс Student, заданный фамилией, именем, возрастом
+и средним баллом. Включите в описание класса методы: вывода
+информации о студенте на экран, проверки, является ли студент
+отличником (средний балл больше 4.5), и свойство, позволяющее
+установить факультет, на котором учится студент.
+class Student:    
+    def __init__(self, surname, name, age, mean):
+        self.surname = surname
+        self.name = name
+        self.age = age
+        self.mean = mean
+        self._faculty = ''
+        
+    def info(self):
+        return self.__dict__        
+        
+    def excellent(self):
+        return self.mean > 4.5 
+    
+    @property
+    def faculty(self):
+        return self._faculty
+    
+    @faculty.setter
+    def faculty(self, faculty):
+        self._faculty = faculty
+
+a = Student('Головкина', 'Анна', 18, 4.6)
+print(a.info())
+
+a.faculty = 'ИТиАБД'
+
+print(a.info())''')
+
+def vsapsu():
+    print('''Написать функцию, которая принимает на вход список чисел и сортирует его по убыванию с помощью алгоритма сортировки вставками. Функция должна возвращать отсортированный список.
+def insertion_sort(reverse=True):
+    arr = []
+    while True:
+        elem = input()
+        if elem != None and elem != '':
+            arr.append(int(elem))
+        else:
+            break
+            
+    for i in range(1, len(arr)):
+        key = arr[i]
+        j = i - 1
+        while j >= 0 and ((not reverse and arr[j] > key) or (reverse and arr[j] < key)):
+            arr[j + 1] = arr[j]
+            j -= 1
+        arr[j + 1] = key
+    return arr
+
+insertion_sort()''')
+
+    
+#22
+def akvpn():
+    print('''Напишите лямбда-функцию, которая умножает заданное число на 7 и вычитает из него 3, переданное в качестве аргумента.
+a = [1, 2, 3, 4, 5, 6]
+expression = list(map(lambda x: x*7-3, a))
+
+expression''')
+
+def lpschts():
+    print('''Найдите сумму всех чисел в заданном списке целых чисел с помощью лямбда-функции.
+from functools import reduce
+arr = list(np.random.randint(-100, 100, 10))
+print(arr, sum(arr))
+a = reduce(lambda x, y: x+y, arr)
+a''')
+
+def lpschz():
+    print('''Извлечь элементы списка, которые больше заданного числа, с помощью лямбда-функции.
+arr = list(np.random.randint(-100, 100, 10))
+print(arr)
+val = int(input())
+a = list(filter(lambda x: x > val, arr))
+a''')
+
+def chpyake():
+    print('''Дан стек. Необходимо найти сумму всех элементов, которые являются простыми числами.
+import copy
+
+class Node:
+    def __init__(self, data):
+        self.data = data
+        self.next = None
+
+class Stack:
+    def __init__(self):
+        self.head = None
+
+    def is_empty(self):
+        return self.head is None
+
+    def push(self, item):
+        new_node = Node(item)
+        new_node.next = self.head
+        self.head = new_node
+
+    def pop(self):
+        if self.is_empty():
+            return None
+        else:
+            popped_item = self.head.data
+            self.head = self.head.next
+            return popped_item
+        
+    def find_prime(self):
+        
+        def is_prime(a):
+            if a==1:
+                return False
+            if a % 2 == 0:
+                return a == 2
+            d = 3
+            while d * d <= a and a % d != 0:
+                d += 2
+            return d * d > a
+        
+        a = []
+        
+        temp_stack = Stack()
+
+        temp_stack = copy.deepcopy(self)
+
+        while not temp_stack.is_empty():
+            item = temp_stack.pop()
+            if is_prime(item):
+                a.append(item)
+
+        return sum(a)
+        
+
+    def peek(self):
+        if self.is_empty():
+            return None
+        else:
+            return self.head.data
+
+    def __str__(self):
+        current = self.head
+        stack_str = ""
+        while current:
+            stack_str += str(current.data) + " → "
+            current = current.next
+        return stack_str.rstrip(" → ")
+
+stack = Stack()
+
+for i in [x for x in np.random.randint(0, 100, 10)]:
+    stack.push(i)
+    
+print(stack)
+
+stack.find_prime()''')
+
+#23
+def igpkd():
+    print('''#Создайте класс «Книга» с атрибутами название, автор и год издания.
+Напишите методы для вывода информации о книге в виде «Книга
+'{название}' автора {автор}, издана в {году}». Используйте магический
+метод __eq__ для сравнения двух книг по году издания
+class Book:    
+    def __init__(self, name, author, year):
+        self.name = name
+        self.author = author
+        self.year = year
+        
+    def info(self):
+        return f'Книга "{self.name}" автора {self.author}, издана в {self.year} году' 
+    
+    @classmethod
+    def __verify_data(cls, other):
+        return other.year
+    
+    def __eq__(self, other):
+        sc = self.__verify_data(other)
+        return self.year == sc
+
+a = Book('Преступление и наказание', 'Достоевский Ф.М.', 1866)
+b = Book('Капитанская дочка', 'Пушкин А.С.', 1836)
+c = Book('Война и мир', 'Толстой Л.Н.', 1863)
+d = Book('Палата №6', 'Чехов А.П.', 1892)
+f = Book('Казаки', 'Толстой Л.Н.', 1863)
+
+a.info(), b.info(), c.info(), d.info(), f.info()
+
+a == b
+
+c == f''')
+
+def vsapss():
+    print('''#Написать функцию, которая принимает на вход список строк
+и сортирует его по длине строк с помощью алгоритма сортировки
+выбором. Функция должна возвращать отсортированный список. 
+
+def selection_sort(arr, reverse=False):
+    n = len(arr)
+    for i in range(n):
+        min_idx = i
+        for j in range(i + 1, n):
+            if reverse:
+                if len(arr[j]) > len(arr[min_idx]):
+                    min_idx = j
+            else:
+                if len(arr[j]) < len(arr[min_idx]):
+                    min_idx = j
+        arr[i], arr[min_idx] = arr[min_idx], arr[i]
+    return arr
+
+a = ['1', '12', '123', '1234', '12345', '123456']
+
+selection_sort(a, True)''')
+
+#24    
+def sokvv():
+    print('''#Опишите класс BankAccount, заданный номером счета, балансом
+и владельцем. Включите в описание класса методы: вывода информации
+о банковском счете на экран, проверки, достаточно ли денег на счете
+для выполнения операции, и свойство, позволяющее установить тип
+валюты, в которой открыт счет
+class BankAccount:    
+    def __init__(self, number, balance, holder):
+        self.number = number
+        self.balance = balance
+        self.holder = holder
+        self._currency = ''
+        
+    def info(self):
+        return self.__dict__        
+        
+    def enough(self, cost):
+        return self.balance >= cost 
+    
+    @property
+    def currency(self):
+        return self._currency
+    
+    @currency.setter
+    def currency(self, currency):
+        self._currency = currency
+
+a = BankAccount(55362036, 201030405020, 'GOLOVKINA ANNA')
+print(a.info())
+
+a.currency = 'USD'
+
+print(a.info())''')
+
+def psaps():
+    print('''#Написать функцию, которая принимает на вход список дат и сортирует
+его по возрастанию с помощью алгоритма сортировки пузырьком.
+Функция должна возвращать отсортированный список
+def bubble_sort(arr, reverse=True):
+    n = len(arr)
+    
+    for i in range(n):
+        for j in range(n - i - 1):
+            if not reverse:
+                if (arr[j] > arr[j + 1]):
+                    arr[j], arr[j + 1] = arr[j + 1], arr[j]
+            else:
+                if (arr[j] < arr[j + 1]):
+                    arr[j], arr[j + 1] = arr[j + 1], arr[j]
+    return arr
+
+a = ['2004-06-29', '2005-01-17', '2004-02-03', '2004-05-26', '1980-06-18', '1978-02-18', '1953-10-24', '1951-08-31', '2011-01-09']
+
+bubble_sort(a)
+''')
```

### Comparing `podval-3.4/podval/podval.py` & `podval-3.5/podval/podval.py`

 * *Files identical despite different names*

