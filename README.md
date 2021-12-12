# PythonStudyNotes :snake:
# Topics with some information to repeat or remember the theme 👨‍💻
![Alt-here we go](https://sun9-45.userapi.com/impg/UgUbvLP-EjVueaNLdjM4kaSdewuAQ2sffMrsJg/yBFjglfgQtY.jpg?size=640x823&quality=96&sign=8ced8c778aaef4554e382da0bbe2a014&type=album)

- [Syntax](https://github.com/EgorNesterenkoSPB/PythonStudyNotes#Syntax)

## Syntax

## Строки

`message = 'Hello "Python" World!'`

`print(message) `

// Hello "Python" World!


Метод `.title()` преобразует первый символ каждого слова в строке к верхнему регистру:

`message = 'hello python'`

`print(message.title())`

// Hello Python

`.upper()`  и  `.lower()` преобразовывает все символы строки к верхнему и нижнему регистру:

`message = 'hello python'`

`print(message.upper())`

// HELLO PYTHON

`message = 'HEllo'`

`print(message.lower()) `

`hello`

Конкатенация – объединения строк:

`message = 'HEllo'`

`secondMessage = "user"`

`outputMessage = message + " " +  secondMessage`

`print(outputMessage)`

// HEllo user

Табуляция и разрывы строк:

`message = "hello \nuser"`

`print(message)`

// hello 
User

`message = "hello \tuser"`

`print(message)`

// hello   user

Удаление пробелом с с начала и конца строки:

`.rstrip()` – удаляет пробел в конце строки 

`message = "hello "`

`currentMessage = message.rstrip()`

`.lstrip()` – удаляет пробел с начала строки 

`.strip()` – удаляет пробела с начала и конца строки

## Числа

Возвести в степень:

`3**2`

// 9

Чтобы преобразовать нестроковое значение в строковое – str()
`message = "hello "`

`userID = 503`

`currentMessage = message + str(userID)`

`print(currentMessage)`

// hello 503

Чтобы поставить комментарий - #

## Списки

Пустой список – `array = []`


Чтобы возвратить элементы с конца списка – `array[-1]` – данный пример выведет последний элемент. Списка

Метод  `.insert()` добавляет новый элемент в указанную позицию 

`array = ["Egor","Nesterenko"]`

`array.insert(1,"Hello")`

`print(array)`

// ['Egor', 'Hello', 'Nesterenko']

Метод del удаляет элемент из списка:

`array = ["Egor","Nesterenko"]`
`del array[1]`

`print(array)`

// ['Egor']

Метод `.pop()` удаляет последний элемент из списка:
`array = ["Egor","Nesterenko"]`

`lastElement = array.pop()`

`print(lastElement)`

`print(array)`

`// Nesterenko`

// ['Egor']

Также в скобках можно указать определенный индекс элемента в списке для его удаления

Метод `.remove(элемент)` – удаляет элемент если он находится в списке

Метод `.sort()` сортирует список в алфавитном порядке

Чтобы отсортировать список в обратном алфавитном порядке - `.sort(reverse=True)`

Метод `sorted()` позволяет предоставить список в определенном порядке не изменяя список

`array = ["Egor","Nesterenko","Adam"]`

`print(sorted(array))`

`print(array)`

// ['Adam', 'Egor', 'Nesterenko']
 
['Egor', 'Nesterenko', 'Adam']

Метод `.reverse()` делает список в обратном порядке 

Метод `len(список)` определяет длину списка

## Цикл for:

`array = ["Egor","Nesterenko","Adam"]`

`for name in array :`

   ` print("hi " + name)`
    
`print("end")`

// hi Egor

hi Nesterenko

hi Adam

end

Чтобы начать писать код после цикла – нужно убрать пробел

Функция range()

`For value in range(1,5):`

 `Print(value)`
 
//1

2

3

4

Последний элемент исключается

Функция `list(range(…))` создает список

`Numbers = list(range(1,6))`

`Print(numbers)`

//[1,2,3,4,5]

## Генерация числовых последовательностей:

`Numbers = list(range(1,11,2))`

` Print(numbers)`
 
//[2,4,6,8,10]

Минимум списка : `min(array)`

Максимум списка: `max(array)`

Сумма списка: `sum(array)`

Генерирования списка в одну строку:

`Squares = [value**2 for value in range(1,11)]`

## Срез - это подмножество списка

`array = ["Egor","Nesterenko","Adam"]`

`print(array[0:2])`

// ['Egor', 'Nesterenko']

`array = ["Egor","Nesterenko","Adam"]`

`print(array[:3])`

// ['Egor', 'Nesterenko', 'Adam']

Без указания начального индекса – python начинает с начала, тоже применимо для если не указан последний индекс то метод идет до конца

Копирование списка:

`array = ["Egor","Nesterenko","Adam"]`

`secondArray = array[:]`

`print(secondArray)`

// ['Egor', 'Nesterenko', 'Adam']

## Кортежи - это список элементов который не может изменяться

`Dimensions = (200,50)`

`Print(Dimensions[0])`

//200

Замена значений в кортеже:

`Dimensions = (200,50)`

`Dimensions = (400,10)`

`Print(Dimensions)`

//400

10


## Условия

`Age = 18`

`If age > 15 :`

`Print(…)`

----------

`If age > 16 :`

`Print()`

`Else:`

`Print()`

----------

`If age > 10 :`

`Print()`
 
`Elif age > 15 :`

`Print()`
 
`Else:`

`Print()`

-----------

При проверки двух условий ставится and или or

Проверить значение например в списке можно с помощью in :

`array = ["Egor","Nesterenko","Adam"]`

`print("Egor" in array)`

// True

`array = ["Egor","Nesterenko","Adam"]`

`print("Egor" not in array)`

// False

Проверка на пустой список: возвращает true если в списке есть хоть один элемент

`array = []`

`if array :`

  ` print("not empty")`
`else :`

   ` print("empty")`
    
//empty

## Словарь

`Alien = {“color”: “green”, ”points”: 5}`

`Print(alien[“points”])`

// 5

Добавление ключ – значения в словарь:

`Alien[“heads”] = 3`

Создание пустого словаря:

`Alien = {}`

Изменения значения в словаре при уже существующем с ключом “color”: 

`Alien[“color”] = “red”`

Удаление ключа соответственно вместо со значением:

`Del alien[“color”]`

Перебор всех пар ключ-значение через цикл:

`For key, value in user.items() : `

`Print(…)`

`Print(…)`


Перебор всех ключей в словаре:

`For name in array.keys() : `

	Print(…)`

Или можно просто без `.keys()` :

`For name in dictionary :`

 `Print()`
 
Выводить тоже будет ключи с словаре

Проверка ключа в списке :

`If “Egor” not in dictionary.keys() : `

 ` Print()`

Сортировочный метод получения элементов ключей в алфавитном порядке:

`For name in sorted(dictionary.keys()) :`

	 `Print(…)`

Перебор всех значений в словаре:

`For language in languages.values() : `

 `Print(…)`

Вывод уникальных значений из словаря:

`For name in set(names.value()) :`

 `Print(name)`

## Словарь в списке:

`Aliens = []`

`For alien in range(10) : `

 `newAlien = {“color” : “red”, “point” : 10}`
 
 `alliens.append(newAlien)`

`for alien in aliens :` 

 `alien[“color”] = “yellow”`


## Список в словаре:

`Pizza = {“cost”:100, “toppings”: [“cheese”, “mushrooms”]}`

`For topping in pizza[“toppings”] : `

 `Print(topping)`

-------------------------

`Dictionary = {“Egor”: [“C++”, “Swift”], “Danil”: [“Java”, “Python”]}`

`For name, languages in dictionary.items() : `

 `For language in languages : `
 
  `Print(language)`


## Словарь в словаре:

`Users = {“Egor”: {“home”: ”Russia”, ”age”:  16}, “Danil”: {“home”: ”Spain”, ”age”: 20}}`

`For user, userInfo in users.items() :`

 `Home = userInfo[“home”]`
 
 `Age = userInfo[“age”]`
