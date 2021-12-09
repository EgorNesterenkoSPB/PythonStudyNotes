# PythonStudyNotes :snake:
# Topics with some information to repeat or remember the theme 👨‍💻
![Alt-here we go](https://sun9-45.userapi.com/impg/UgUbvLP-EjVueaNLdjM4kaSdewuAQ2sffMrsJg/yBFjglfgQtY.jpg?size=640x823&quality=96&sign=8ced8c778aaef4554e382da0bbe2a014&type=album)

- [Syntax](https://github.com/EgorNesterenkoSPB/PythonStudyNotes#Syntax)

## Syntax

## Строки

`message = 'Hello "Python" World!'`

`print(message) `

`// Hello "Python" World!`


Метод `.title()` преобразует первый символ каждого слова в строке к верхнему регистру:

`message = 'hello python'`

`print(message.title())`

`// Hello Python`

`.upper()`  и  `.lower()` преобразовывает все символы строки к верхнему и нижнему регистру:

`message = 'hello python'`

`print(message.upper())`

`// HELLO PYTHON`

`message = 'HEllo'`

`print(message.lower()) `

`hello`

Конкатенация – объединения строк:

`message = 'HEllo'`

`secondMessage = "user"`

`outputMessage = message + " " +  secondMessage`

`print(outputMessage)`

`// HEllo user`

Табуляция и разрывы строк:

`message = "hello \nuser"`

`print(message)`

`// hello `
`User`

`message = "hello \tuser"`

`print(message)`

`// hello   user`

Удаление пробелом с с начала и конца строки:

`.rstrip()` – удаляет пробел в конце строки 

`message = "hello "`

`currentMessage = message.rstrip()`

`.lstrip()` – удаляет пробел с начала строки 

`.strip()` – удаляет пробела с начала и конца строки

## Числа

Возвести в степень:

`3**2`

`// 9`

Чтобы преобразовать нестроковое значение в строковое – str()
`message = "hello "`

`userID = 503`

`currentMessage = message + str(userID)`

`print(currentMessage)`

`// hello 503`

Чтобы поставить комментарий - #

## Списки

Пустой список – `array = []`


Чтобы возвратить элементы с конца списка – `array[-1]` – данный пример выведет последний элемент. Списка

Метод  `.insert()` добавляет новый элемент в указанную позицию 

`array = ["Egor","Nesterenko"]`

`array.insert(1,"Hello")`

`print(array)`

`// ['Egor', 'Hello', 'Nesterenko']`

Метод del удаляет элемент из списка:

`array = ["Egor","Nesterenko"]`
`del array[1]`

`print(array)`

`// ['Egor']`

Метод `.pop()` удаляет последний элемент из списка:
`array = ["Egor","Nesterenko"]`

`lastElement = array.pop()`

`print(lastElement)`

`print(array)`

`// Nesterenko`

`// ['Egor']`

Также в скобках можно указать определенный индекс элемента в списке для его удаления

Метод `.remove(элемент)` – удаляет элемент если он находится в списке

Метод `.sort()` сортирует список в алфавитном порядке

Чтобы отсортировать список в обратном алфавитном порядке - `.sort(reverse=True)`

Метод `sorted()` позволяет предоставить список в определенном порядке не изменяя список

`array = ["Egor","Nesterenko","Adam"]`

`print(sorted(array))`

`print(array)`

` // ['Adam', 'Egor', 'Nesterenko']`
 
`['Egor', 'Nesterenko', 'Adam']`

Метод `.reverse()` делает список в обратном порядке 

Метод `len(список)` определяет длину списка

