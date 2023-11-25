# Тема 8. Введение в ООП
Отчёт по теме #8 выполнил:

• Непеин Никита Сергеевич

• ПИЭ-21-1
| Задание | Лаб_раб | Сам_раб |
| --- | --- | --- |
| Задание 1 | + | + |
| Задание 2 | + | + |
| Задание 3 | + | + |
| Задание 4 | + | + |
| Задание 5 | + | + |

# Лабораторная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/f276f136-fcb3-43b5-8e30-a32a9b52a9b9)
Листинг кода с комментариями:

class Car:  # определяем класс Car
    def __init__(self, make, model):  # Конструктор класса, вызывается при создании нового объекта класса
        self.make = make  # атрибут объекта - марка
        self.model = model  # атрибут объекта - модель


my_car = Car("Toyota", "Camry")  # создаем объект my_car класса Car с указанными параметрами

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/716790d2-4914-44fa-84ac-d52654becb8d)
Листинг кода с комментариями:

class Car:  # определяем класс Car
    def __init__(self, make, model):  # Конструктор класса, вызывается при создании нового объекта класса
        self.make = make  # атрибут объекта - марка
        self.model = model  # атрибут объекта - модель

    def drive(self):  # Метод класса, представляющий действие вождения
        print(
            f"Driving the {self.make} {self.model}")  # Выводит сообщение о вождении автомобиля с указанием марки и
        # модели


my_car = Car("Toyota", "Camry")  # создаем объект my_car класса Car с указанными параметрами
my_car.drive()  # Вызываем метод drive() для объекта my_car,
     # выводя сообщение о вождении с указанием марки и модели автомобиля

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/f2c5cee1-b420-406a-a512-f7c915f1583d)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/f5e68cf9-71f7-4047-86ec-8c3228edd9ab)
Листинг кода с комментариями:

class Car:  # определяем класс Car
    def __init__(self, make, model):  # Конструктор класса, вызывается при создании нового объекта класса
        self.make = make  # атрибут объекта - марка
        self.model = model  # атрибут объекта - модель

    def drive(self):  # Метод класса, представляющий действие вождения
        print(
            f"Driving the {self.make} {self.model}")  # Выводит сообщение о вождении автомобиля с указанием марки и
        # модели


my_car = Car("Toyota", "Camry")  # создаем объект my_car класса Car с указанными параметрами
my_car.drive()  # Вызываем метод drive() для объекта my_car,


# выводя сообщение о вождении с указанием марки и модели автомобиля

class ElectricCar(Car):  # Создаем подкласс ElectricCar
    def __init__(self, make, model, battery_capacity):  # Конструктор подкласса
        super().__init__(make, model)  # Вызываем конструктор родительского класса с передачей марки и модели
        self.battery_capacity = battery_capacity  # Инициализируем новый атрибут battery_capacity

    def charge(self): # Метод charge для зарядки электрического автомобиля
        print(f"Charging the {self.make} {self.model} with {self.battery_capacity} kWh")  # Выводим сообщение о
        # зарядке с указанием марки, модели и емкости батареи


my_electric_car = ElectricCar("Tesla", "Model S", "75")  # Создаем объект my_electric_car подкласса ElectricCar с
    # указанными параметрами, включая емкость батареи
my_electric_car.drive()  # Вызываем унаследованный метод drive() для объекта my_electric_car, выводящий сообщение о вождении
my_electric_car.charge()  # Вызываем метод charge() для объекта my_electric_car, выводя сообщение о зарядке с указанием марки, модели и емкости батареи

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2849ddf0-cd3e-405d-aac4-44294c2ed479)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/d40140b1-8cfa-4687-832d-f19a6191e198)
Листинг кода с комментариями:

class Car:  # определяем класс Car
    def __init__(self, make, model):  # Конструктор класса, вызывается при создании нового объекта класса
        self._make = make   # Защищенный атрибут
        self.__model = model    # Приватный атрибут

    def drive(self):    # Метод, выводящий сообщение о вождении с использованием атрибутов марки и модели
            print(f"Driving the {self._make} {self.__model}")  # Используем f-строку для вывода сообщения о вождении автомобиля,
# вставляя значения защищенного атрибута _make и приватного атрибута __model


my_car = Car("Toyota", "Camry")  # Создаем объект my_car класса Car с маркой "Toyota" и моделью "Camry"
print(my_car._make) # Доступ в защищенному атрибуту, так как он доступен извне класса
print(my_car.__model) # Ошибка! Приватный атрибут недоступен, так как он доступен внутри класса
my_car.drive()

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/5ca88b43-d9a1-4661-9475-100784611929)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/5f88940c-e328-4a9e-b42f-2d6e1dc08173)
Листинг кода с комментариями:

# Определяем базовый класс Shape с абстрактным методом area, который должен быть переопределен в производных классах
class Shape:
    def area(self):
        pass


# Производный класс Rectangle, наследуемый от Shape
class Rectangle(Shape):
    def __init__(self, width, height):
        # Инициализируем атрибуты объекта - ширину и высоту прямоугольника
        self.width = width
        self.height = height

    def area(self):
        # Переопределяем метод area для прямоугольника, возвращая произведение ширины на высоту
        return self.width * self.height


# Производный класс Circle, также наследующий от Shape
class Circle(Shape):
    def __init__(self, radius):
        # Инициализируем атрибут объекта - радиус круга
        self.radius = radius

    def area(self):
        # Переопределяем метод area для круга, возвращая площадь по формуле pr^2
        return 3.14 * self.radius * self.radius


# Создаем объекты классов Rectangle и Circle
rectangle = Rectangle(5, 7)
circle = Circle(4)

# Вызываем метод area() для каждого объекта и выводим результаты
print(rectangle.area())  # площадь прямоугольника
print(circle.area())  # площадь круга

# Самостоятельная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/9da340db-7f0d-4140-8f6c-92c8f6a37700)
Вывод: создаем класс People, который представляет собой модель человека с атрибутами name и age. В классе определен метод display_info, который выводит информацию о человеке в консоль. Затем создается объект класса People с именем  и возрастом, и вызывается метод display_info для вывода информации о данном человеке в консоль.

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/9824903c-19c6-4020-b173-8a171f77ebaa)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/ab84bb26-d9e0-47cf-8dfa-16dca446b153)
Вывод: определяем класс People, представляющий человека с атрибутами name, age, city и grades . Класс имеет методы display_info для вывода основной информации о человеке и display_grades для отображения данных об оценках ученика.
Затем создается объект класса People с конкретными значениями, и вызываются методы для вывода информации о человеке и его оценках в консоль

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/dd174ba2-9606-4c3a-9e50-5bd4bad0d4d1)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/199a85a6-79a0-409d-8e66-343f8cecce30)
Вывод: Теперь класс Student является подклассом класса People с помощью метода super() в инициализаторе подкласса, чтобы вызвать инициализатор суперкласса и сохранить общую информацию о студенте. Затем добавляем метод display_grades для класса Student. Создаем объект one_student типа Student, и вызываем методы для вывода информации о студенте и его оценках в консоль

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/611be9ab-b415-47b1-a7a4-53b096e4f13c)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/dcf296bd-46c6-4d1f-bfef-093b066a0bd0)
Вывод: сделали защищенным атрибут self._grades = grades.

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/0f445bad-56ab-4c6e-921a-83432e28f0cf)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/7824e328-fc15-4b1d-b194-e8cce63b2f6d)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/0592ad60-b4d4-42ff-8d41-2fd8e06eca0e)
Вывод: добавили метод study в оба класса, чтобы показать полиморфизм, и теперь оба класса имеют метод study, и мы можем вызвать этот метод на объектах обоих классов. Это демонстрирует полиморфизм, где метод study реализуется по-разному в каждом классе, но имеет общий интерфейс
