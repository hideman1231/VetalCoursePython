# Основная работа в программировании - манипуляция с данными (у нас есть какие-то данные и мы что-то с ними делаем).

Вот простой пример:
- У нас есть какие-то данные
- ![](./images/image%20(31).png?raw=true)
- Мы нажимаем на 3 кнопки
- ![](./images/image%20(32).png?raw=true)
- Данные поменялись. Это могло быть все что угодно, математические вычесления 
(меняем существующие данные) или же просто подменна на другие данные 
(мы берем данные в другом месте, не меняя старые)
- ![](./images/image%20(33).png?raw=true)

# Как в Python можно хранить данные и на какие виды они делятся?

Вот ОСНОВНЫЕ типы данных в Python:

- Числа (Numbers).
```python 
# Основные числовые данные:
number = 10 # целый числа
pi = 3.14 # дробовые числа
```

Мы в "number" записали число 10, "number" просто название нашей переменной, это может быть 
почти любое слово, которое поддерживает язык. Теперь мы можем использовать наши переменные ("number" и "pi")

```python 
print(number + pi) # 13.14
# Функция print выводит результат на экран когда мы запускаем скрипт

result = number - pi # Или присвоить нашей переменой результат вычисления. 
# result = 6.859999999999999 (почему так происходит, пока не важно)
```

Подробное про операции с числами и другими типами данных мы обусдим на следющем уроке :)

- Строки (Strings)

    Строка в Python - это последовательность символов (абсолютно любые символы)
```python 
str = '' # пустая строка
str1 = 'some text...'
str2 = "some text..."
str3 = """some text..."""

# Из примеров видно, что строки можно объявлять несколькими способами, c помощью: 
- ' ' (одинарные кавычки)
- " " (двойные кавычки)
- ''' ''' (три одинарные кавычки)
- """ """ (три двойные кавычки)
```

Почему нельзя было сделать один вид кавычок!? Иногда у нас могу быть случаи
когда в строке нужно отобразить кавычки. Вот пример:

```python 

str = '3 != "3" '
print(str) # выведет: 3 != "3"

str = '3 != '3' ' # будет ошибка!
```

- Список (List)
    
    Список в Python - упорядоченая коллекция, которая хранит в себе абсолютно любыи данные

```python 
lst1 = [] # объявлем через квадратные скобки, пустой список

one = 1
twenty_five = 25
lst2 = [one, 'hello 2', [twenty_five, 1, ['python', {'key': 'value'}, 'abc']], twenty_five]
print(lst) # выведет [1, 'hello 2', [25, 1, ['python', {'key': 'value'}, 'abc']], 25]
```

- Словарь (Dictionary)

    Словарь в Python - это не упорядоченая коллекция, в котором данные хранятся в виде `ключ: значение`

```python
phones = [0936596412, 0789996123]

data = {'age': 21, 'name': 'Danya', 'phones': phones} # объявляется через фигурные скобки
print(data) # выведет: {'age': 21, 'name': 'Danya', 'phones': [0936596412, 0789996123]}
```

- Кортеж (Tuple)

    Кортеж в Python - упорядоченая коллекция, которая хранит в себе абсолютно любыи данные 
  (очень похож на Список, в чем их разница узнаем позже)

```python 
tuple0 = () # пустой Кортеж
tuple1 = (1, 2) 
tuple2 = 1, 2 # скобки не обязательные
tuple2 = 1, # это тоже будет Кортежом из одного элемента!
```

- Множество (Set)

    Множество в Python - это не упорядоченая коллекция, которая хранит в себе только уникальные элементы.
  (хранит в себе только Строки, Числа и Кортеж)

```python 
set0 = {} # Не Множество, а Словарь, чтобы объявить пустое Множество нужно использовать функцию set() 
set1 = set() # пустое Множество 

one = 1
set2 = {one, 2, 2, '1', 3, 10, 1}
print(set2) # выведет: {'1', 2, 3, 1, 10}
# Обрати внимание в нем удалились дубликаты, но вывод Множества всегда будет в случайном порядке

set3 = {1, 2, 2, '1', 3, {'key', 'value'}} # будет ошибка, если поместить, например Словарь
```

- Булевы значения

    Булевы значения в Python это две константы `True` и `False`

```python 
true = True
false = False
```

# Домашнее Задание

1) Сделать Список в котором хранятся:
   - два Кортежа с значениями от 1 до 10
   - словарь с биографией (минимум 3 ключа, один из них должен быть Лист)
   - Булевое значение
   - пустое Множество
   - Лист с одним Картежом из первого пункта и 3 строки в котором есть строки (разные комбинации)
2) Записать этот список в переменую `result` и вывести его
