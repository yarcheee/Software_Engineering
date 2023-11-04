# Тема 5. Базовые коллекции: множества, списки
Отчёт по теме #5 выполнил:

• Непеин Никита Сергеевич

• ПИЭ-21-1
| Задание | Лаб_раб | Сам_раб |
| --- | --- | --- |
| Задание 1 | + | + |
| Задание 2 | + | + |
| Задание 3 | + | + |
| Задание 4 | + | + |
| Задание 5 | + | + |
| Задание 6 | + | - |
| Задание 7 | + | - |
| Задание 8 | + | - |
| Задание 9 | + | - |
| Задание 10 | + | - |

# Лабораторная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/ca169461-99a1-4012-a692-7395743c8f68)

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/0efa0c88-3345-46ad-844b-554c33f3d8f7)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2177603c-57fd-463d-bc23-8dca89fe9c5c)

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/8198305b-2fa5-474d-87eb-a696f99f0070)

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/8b4f34a5-ce5e-4adb-bfba-cb63c96ee807)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/d7e5b06c-d197-4197-92b3-39b32aa89702)

6.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/70928527-1ec0-4073-9163-e411c2df97d0)

7.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/63caff78-c4c8-4b02-9f65-262df6edba01)

8.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/5aac913e-b6f8-4b76-bc92-d8e51b7f2a38)

9.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/b07ddf27-4932-444f-be9c-7cedcc0e2d2f)

10.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/dde69e99-5ded-4bb4-8f2f-5062ceef7a61)

# Самостоятельная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/dc5ef436-482c-40ae-921f-dbb2a75f00e3)
Вывод:checks = [] Создаем список checks и заполняем его чеками
total_checks = len(checks) С помощью функции len() находим длину списка checks и узнаем сколько чеков было выдано. Результат сохраняем в переменной total_checks
unique_visitors = len(set(checks)) Создаем множество (set) из списка checks, что автоматически убирает повторяющиеся элементы. Затем снова используем len() для определения количества уникальных посетителей ресторана
most_frequent_worker = max(set(checks), key=checks.count) Создаем множество (set) из списка checks, чтобы убрать повторяющиеся элементы, а затем используем max() с аргументом key и находим элемент с наибольшим количеством в списке. Это определяет код с наибольшим количеством повтора
print(): Используем функцию print() для вывода результатов на экран. Каждая строка print() выводит определенный ответ

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/cf9090b6-68e1-4e0f-b69c-cd3087065e43)
Вывод: results = []: создаем список results и заполняем его результатами бега
best_three = sorted(results)[:3]: Создаем переменную best_three и используем функцию sorted() для сортировки списка results по возрастанию. Затем мы используем срез [:3], чтобы взять первые три отсортированных значения, которые будут тремя лучшими результатами
worst_three = sorted(results)[-3:]: Создаем переменную worst_three и снова используем функцию sorted() для сортировки списка results по убыванию. Затем мы используем срез [-3:], чтобы взять последние три отсортированных значения, которые будут тремя худшими результатами.
above_ten = [result for result in results if result >= 10]: Создаем переменную above_ten и используем список-выражение для фильтрации списка results. Мы оставляем только те результаты, которые больше или равны 10.
print(): Используем функцию print() для вывода результатов на экран. Каждая строка print() выводит определенный ответ

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/fc46ab8d-e546-4722-86dc-3ee8a2f4cb79)
Вывод:import math Импортируем модуль math, который содержит математические функции
one = [12, 25, 3, 48, 71], two = [5, 18, 40, 62, 98], three = [4, 21, 37, 56, 84] - Создаем три списка с длинами сторон треугольников
def triangle_area(a, b, c) -  Определяем функцию triangle_area, которая принимает три аргумента (длины сторон треугольника)
s = (a + b + c) / 2 - Вычисляем полупериметр треугольника
return math.sqrt(s * (s - a) * (s - b) * (s - c)) -  Используя формулу Герона, вычисляем площадь треугольника и возвращаем ее.
for sides in [one, two, three] - Запускаем цикл, который будет выполнять следующий код для каждого из трех списков длин сторон.
area = triangle_area(min(sides), max(sides), max(sides)) - Вычисляем площадь треугольника, передавая в функцию triangle_area минимальное и максимальное значение из текущего списка длин сторон
print(f"Площадь треугольника: {area:.2f}") - Выводим результат в формате с двумя десятичными знаками

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/8dde4251-108d-43f2-bd61-4dc51e86fbf1)
Вывод:
Создаем список grades с оценками студента.
grades = [grade for grade in grades if grade != 2] - Создаем новый список, используя генератор списка (list comprehension), чтобы перебрать все оценки в исходном списке и включить их в новый список, только если оценка не равна 2
grades = [4 if grade == 3 else grade for grade in grades] - Мы снова создаем новый список с использованием генератора списка. В этом случае мы заменяем оценки 3 на 4, а все остальные оценки остаются без изменений
print(grades) - Выводим измененный список оценок на экран

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/4a2f6618-e2a8-4cbb-9976-6057f4080efa)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/75e374b1-fb79-4a8a-abf9-b56717b4d094)
Вывод:
определяем функцию create_set, которая создает множество с учетом указанного правила
В основной части кода, у нас есть три списка с натуральными числами (list_1, list_2, list_3)
Мы вызываем функцию create_set для каждого из этих списков, чтобы получить соответствующие множества (result_set_1, result_set_2, result_set_3)
Полученные множества содержат числа и строки, удовлетворяющие указанным условиям
И выводим эти множества на экран

























































