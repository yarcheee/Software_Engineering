# Тема 10. Декораторы и исключения
Отчёт по теме #10 выполнил:

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
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/158398c2-2cf4-45bb-9ad9-408aee32d71c)

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/8561a496-c19c-4d8d-a491-5de9a15be4ed)

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/a6c801f6-0783-4b1b-ac61-e8514e67f332)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/eafb6118-54cd-47f3-86dd-83ddfa7af311)

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/14aa1081-5346-4155-89f5-36a41b2e8f72)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/19805e11-e9b4-49bf-be4d-f1884e7a61c7)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/89167093-cd6d-4d5a-a848-2aa9c921abf0)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/9f68e908-1d03-4f9c-a25b-b3dd7282bbc7)

# Самостоятельная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/0a4c2c62-d577-4df5-9a2f-447b1edd420b)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/bfde8331-7d90-4aa1-a392-13b1bf4373dd)

Вывод: Декоратор timing_decorator принимает функцию func и возвращает новую функцию wrapper
Функция wrapper измеряет время начала выполнения функции, вызывает оригинальную функцию (func) с переданными аргументами и измеряет время окончания выполнения.
Затем выводит в консоль время выполнения функции func и возвращает результат её выполнения
Функция fibonacci выводит первые 199 чисел последовательности Фибоначчи. После каждого числа выводится символ новой строки. Каждый вызов print сразу после числа, а не в конце цикла, обеспечивает более наглядный вывод в консоль.
При запуске кода вы увидите вывод чисел Фибоначчи и время выполнения функции fibonacci в консоли

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/d5e81578-4f4e-4812-89f9-25d5c8455e11)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/b9d8e554-7b85-43c8-a442-d4141d5dc4ae)

Вывод: использую конструкцию try-except для обработки исключений. Если файл не найден (FileNotFoundError), программа выводит "Файл не найден". Если в файле есть информация, она выводится на экран. Если файл пустой, вызывается исключение (Exception), и программа выводит "Ошибка: файл пустой". Таким образом, мы обрабатываем ситуацию, когда файл пустой, и предотвращаем возможные ошибки

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/a68498b6-bbf1-418a-b9dd-a5a9dd99338d)

Вывод: Используем try/except для обработки возможных исключений. Ввод пользователя конвертируется в число, и если это не удается (в случае ввода строки или другого неподходящего типа данных), программа перехватывает исключение ValueError и выводит сообщение об ошибке

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/15fe7e69-e7ed-4f9e-9c7a-cacc0957c2dc)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2eae17d0-ad82-4828-a379-0d853708ab87)

Вывод: simple_decorator: Функция, создающая декоратор. Принимает функцию func в качестве аргумента.
wrapper: Внутренняя функция-обертка, которая будет вызываться вместо оригинальной функции. Она выводит информацию о вызове и завершении выполнения функции.
@simple_decorator: Применение декоратора к функциям add_numbers и multiply_numbers.
add_numbers: Простая функция, складывающая два числа.
multiply_numbers: Простая функция, умножающая два числа.
Тесты: вызываем обернутые декоратором функции, и видим, как выводится информация о вызове и завершении выполнения функций

Листинг кода:
# Создаем собственный декоратор simple_decorator
def simple_decorator(func):
    # Внутренняя функция-обертка, которая будет вызываться вместо оригинальной функции
    def wrapper(*args, **kwargs):
        # Выводим информацию о вызове функции
        print(f"Вызвана функция {func.__name__} с аргументами {args} и ключевыми аргументами {kwargs}")
        # Вызываем оригинальную функцию
        result = func(*args, **kwargs)
        # Выводим информацию о завершении выполнения функции
        print(f"Завершена выполнение функции {func.__name__}")
        # Возвращаем результат выполнения оригинальной функции
        return result
    # Возвращаем функцию-обертку в качестве результата декоратора
    return wrapper

# Применяем декоратор к функции add_numbers
@simple_decorator
def add_numbers(a, b):
    return a + b

# Применяем декоратор к функции multiply_numbers
@simple_decorator
def multiply_numbers(x, y):
    return x * y

# Тесты
# При вызове функций информация о вызове и завершении выводится в консоль
result_add = add_numbers(3, 5)
result_multiply = multiply_numbers(2, 4)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/40737625-3919-4d61-9973-5e2451bed028)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2a9227c5-d75a-41b2-8cbe-e00121c91f56)
Вывод: InvalidEmailException: Это собственное исключение, которое наследуется от встроенного класса Exception. Оно инициализируется с невалидным email-адресом
validate_email: Это функция, которая проверяет валидность переданного email-адреса с использованием простой регулярной проверки. Если email невалиден, функция вызывает исключение InvalidEmailException с переданным email-адресом
Тесты: В блоке try мы вызываем функцию validate_email с невалидным email, что приводит к возникновению исключения InvalidEmailException. В блоке except мы обрабатываем и выводим информацию об исключении в консоль
Листинг кода:
import re

# Создаем собственное исключение InvalidEmailException
class InvalidEmailException(Exception):
    def __init__(self, email):
        self.email = email
        super().__init__(f"Невалидный email: {email}")

# Функция, которая проверяет валидность email и вызывает исключение при необходимости
def validate_email(email):
    # Простая регулярная проверка на валидность email-адреса
    if not re.match(r"[^@]+@[^@]+\.[^@]+", email):
        # Вызываем исключение InvalidEmailException
        raise InvalidEmailException(email)

# Пример использования исключения в коде
try:
    # Пытаемся вызвать функцию с невалидным email
    validate_email("invalid.email")
except InvalidEmailException as e:
    # Обрабатываем и выводим информацию об исключении
    print(f"Произошло исключение: {e}")







