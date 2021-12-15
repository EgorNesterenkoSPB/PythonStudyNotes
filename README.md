# PythonStudyNotes :snake:
# Topics with some information to repeat or remember the theme 👨‍💻
![Alt-here we go](https://sun9-45.userapi.com/impg/UgUbvLP-EjVueaNLdjM4kaSdewuAQ2sffMrsJg/yBFjglfgQtY.jpg?size=640x823&quality=96&sign=8ced8c778aaef4554e382da0bbe2a014&type=album)

- [Syntax](https://github.com/EgorNesterenkoSPB/PythonStudyNotes#Syntax)
- [Collections](https://github.com/EgorNesterenkoSPB/PythonStudyNotes#Collections)

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
 
## Ввод данных

Input() – приостанавливает выполнение программы и ждем пока пользователь введет данные

`message = input("Write something:")`

`print(message)`

//Hello there

`Age = int(age)` – преобразование типа строки в тип целого числа

## While

`Pets = [‘cat’, ‘dog’. ’cat’]`

`While ‘cat’ in dog : `

	Pets.remove(‘cat’)`
	
## Функции

`def test() : `

 `  """This is documentation comment"""`
    
 `  print("Test")`
    
`test()`

// Test

`def test(name) : `

   `print("Test " + name)`
    
`test("Egor")`

//Test Egor

`def test(name:int) : `

  ` print("Test " + str(name))`
    
`test(name=50)`

//Test 50

`def test(name:int, age = 20) : `

  ` print("Test " + str(name) + " " + str(age))`
    
`test(name=50)`

// Test 50 20

Важно указывать значения по умолчанию после значений которые еще не определены

Значения по умолчанию также можно изменять при вызове функции

`def test(first:int, second:int) : `

   `return first + second`

`sum = test(first=5,second=5)`

`print(sum)`

//10

Return возвращает значение переменной которая вызывает функцию

`firstArray = [1,2,3]`

`secondArray = []`

`def test(firstArray,secondArray) :`

  ` while firstArray:`
   
        `num = firstArray.pop()`
	
       `secondArray.append(num)`
	
    `print(firstArray)`
    
   ` print(secondArray)`

`test(firstArray,secondArray)`

`print(firstArray)`

//[]

[3, 2, 1]

[]

Чтобы не изменять первый массив можно передать его копию:

`test(firstArray[:],secondArray)`

//[]

[3, 2, 1]

[1, 2, 3]


`def test(*names) :`

   `for name in names:`
   
       ` print(name)`
       
`test("Egor")`

`test("Egor","Danil")`

//Egor

Egor

Danil

Звездочка в аргументе функции может получать любое количество аргументов которе оно преобразует в кортеж

Если функция принимает несколько аргументов то аргумент со звездочкой ставится в конце

`def test(name,age, **test) :`

  ` testing = {}`
  
   ` testing["name"] = name`
    
   ` testing["age"] = age`
    
   ` for key, value in test.items() :`
    
       `testing[key] = value`
	
    `return testing`

`user = test("Egor",20,location = "SPB",university = "Mining")`

` print(user)`

//{'name': 'Egor', 'age': 20, 'location': 'SPB', 'university': 'Mining'}

Две здездочки перед аргументом функции создают словарь

## Модули

Например функция сохраняется в отдельном файле – модуль, а затем импортируется модуль в программу через imports

Модуль – файл с расширением .py

Строка import приказывает Python открыть файл и скопировать все функции из него в программу 

![Alt-example](https://sun9-69.userapi.com/impg/CWba60Rc8bOo8tZ2jpbEKlYSl_Z1oUfG6ZkzHg/s5pVyuwV1Wc.jpg?size=432x126&quality=96&sign=31e652fc50b0a1d4e406e8818234b98f&type=album)

![Alt-example](https://sun9-2.userapi.com/impg/B4xdA53r5YHZlD6mjvPWbgmn3YL9GmY7LZBVvQ/SWd3xgSnIcU.jpg?size=408x230&quality=96&sign=04a2630e584df4b03f1f84c6324c7f23&type=album)

//Hello from another module

`Text from test.py`

Также можно импортировать конкретную функцию из модуля:

`From имяМодуля import имяФункции, имяФункции2`

Чтобы назначить псевдоним функции при импортировании ее – alias (`as` ):

`From имяМодуля import имяФункции as альтернативноеИмя`

Также можно назначить псевдоним для модуля:

`Import имяМодуля as имяПсевдонима`

Чтобы импортировать все функции из модуля – нужно поставить * после слова import:

`From имяМодуля import *`


## Классы
Создание объекта на основе класс – экземпляр

`class Car() :`

  ` """Simple model Car"""`
   
    `def __init__(self,name,color) :`
    
      ` self.name = name`
       
       ` self.color = color`
    
  `  def changeColor(self,newColor) :`
    
`"""Change color car """`

       ` self.color = newColor`
	
       ` print(self.color)`

`toyota = Car("Toyota","Black")`

`print(toyota.color)`

`toyota.changeColor("Yellow") `

//Black

Yellow

При каждом вызове метода связанного с классом автоматически передается self – ссылка на экземпляр, он предоставляет конкретному экземпляру доступ к атрибутам и методам класса

После создания класса и метода внутри класса нужна краткая документация что этот класс делает и что данный метод делает 

Добавляем атрибут по умолчанию:

`def __init__(self,name,color) :`

      ` self.name = name`
       
        `self.color = color`
	
      `  self.mile = 0`

Наследование:

`class ElectroCar(Car) :`

   `def __init__(self, name, color):`
    
    ` #here init values of parent class`
     
      `  super().__init__(name, color)`
	
      `  #here init values of child class`
	
       ` self.charge = 1000`
	
   ` def incrementCharge(self,value) : `
    
       ` self.charge -= value`

`tesla = ElectroCar("Tesla","White")`

`tesla.incrementCharge(200)`

`print(tesla.charge)`

//800

Переопределение методов родителя:

В классе child просто переписываем название метода который хотим изменить у родителя:

`def changeColor(self):`

      ` print("White is the best color")`

`tesla.changeColor()`

//White is the best color

Импортируем класс из модуля: ` from имяМодуля import имяКласса1, имяКласса2`

Импортирование всего модуля: `import имяМодуля`

## Collections

## OrderedDict

Модуль collections позволяет сохранить порядок словаря 

`From collections import OrderedDict`

`Languages = OrderedDict()`

`Languages[“eng”] = “English”`

`Languages[“sp”] = “Spanish”`

`Languages[“ru”] = “Russian”`

`For index, language in Languages.items() : `

`Print(index + “ ” + language)`

//eng English

Sp Spanish

Ru Russian

