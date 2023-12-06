# Тема 11. Итераторы и генераторы
Отчёт по теме #11 выполнил:

• Непеин Никита Сергеевич

• ПИЭ-21-1
| Задание | Лаб_раб | Сам_раб |
| --- | --- | --- |
| Задание 1 | + | + |
| Задание 2 | + | + |
| Задание 3 | + |  |
| Задание 4 | + |  |
| Задание 5 | + |  |

# Лабораторная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/bdba6497-8ddc-4ce2-afd7-0cdbddca0345)

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2e19f868-6123-41d4-889f-832a268ef50b)

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/33f47762-89c5-4caf-aa77-95affca3c1a5)

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/9a426767-8a44-41c9-9d30-371090add0c9)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/6021d502-1b71-41d6-824c-3255e56705a8)

# Самостоятельная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/a2ec99d2-b5b3-4b12-a5ab-76e4844f664d)
Вывод: функция fib принимает аргумент n, который определяет, сколько чисел Фибоначчи нужно сгенерировать
Инициализирует переменные a и b значениями 1, так как последовательность Фибоначчи начинается с 1 и 1
Использует цикл for для итераций от 0 до n - 1
На каждой итерации использует инструкцию yield для возврата текущего значения a
Обновляет переменные a и b так, чтобы следующее число в последовательности было суммой предыдущих двух чисел
Преобразование в список:
Создает переменную fibonacci_sequence, в которую записывается результат вызова list(fib(200)).
Это конвертирует итератор, созданный функцией fib, в список
Вывод в консоль: выводит список fibonacci_sequence в консоль

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/83c45c73-e102-4a86-a1ce-57963d6a194f)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/88edb4b1-34a5-47aa-8c3d-0c0bcfa39797)
Вывод: используем контекстный менеджер with open("fib.txt", "w") as file: для открытия файла "fib.txt" в режиме записи (w)
file.write(str(a) + "\n"), чтобы записать каждое число Фибоначчи с новой строки

























