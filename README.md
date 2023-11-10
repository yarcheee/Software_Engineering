# Тема 6. Базовые коллекции: словари, кортежи
Отчёт по теме #6 выполнил:

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
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/12d954fd-978c-4720-8cfd-e2b10424998b)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/a4dfb569-9bd3-48b3-8bb5-26a176849c09)

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/23f1efd5-2c87-442d-9b72-5b48d7ebc1a9)

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/8a08cc97-58a1-4bf0-894e-44735f1286e3)

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/19d03c7a-1ddf-44a2-9434-b9a457866cd4)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/ac3c10c4-e8ae-4efd-b065-87a47974d3fe)

# Самостоятельная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/4d90b17b-8be7-4591-8341-bd50b48dfe6a)
Вывод: Запрашиваем у пользователя ввод чисел, разделенных пробелом и сохраняем эту строку в переменную user input
Дальше разбиваем введенную строку user_input на список чисел, используя пробелы в качестве разделителей. Потом каждая подстрока преобразуется в целое число (int(num)) и добавляется в новый список (numbers_list).
numbers_tuple = tuple(numbers_list): Преобразует список чисел (numbers_list) в кортеж, сохраняя тот же порядок
далее выводим список numbers_list
также выводим кортеж numbers_tuple

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2367d93a-80f3-4472-a6fc-d324974b6b6d)
Вывод: определяем функцию remove_element_from_tuple, которая принимает два аргумента: my_tuple (кортеж) и element_to_remove (элемент для удаления). Функция использует filter для создания нового кортежа, в котором удалены все вхождения element_to_remove. Затем используем эту функцию для трех кортежей с разными элементами для удаления

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/f88fd5ff-492c-499a-b1ae-6e39c8d832ac)
Вывод: def count_and_sort_digits(input_string) - определяем функцию, которая принимает строку цифр
digit_count = {} - создаем пустой словарь для подсчета встречающихся цифр
for digit in input_string -  цикл, проходящий через каждый символ во входной строке
if digit.isdigit() - проверка, является ли текущий символ цифрой
digit_count[int(digit)] = digit_count.get(int(digit), 0) + 1 - Обновление счетчика для каждой цифры в словаре
result_dict = dict(sorted(digit_count.items(), key=lambda item: item[1], reverse=True)[:3]) - сортировка словаря по убыванию значений и выбор трех самых часто встречаемых чисел
return result_dict – возвращаем словарь с результатами

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/545e7019-41a4-489f-9b67-9efc4658b705)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/55d6785c-9bb7-4b80-8f80-43054f8d20ff)
Вывод: def extract_employee_logs(log_tuple, employee_id)-  Определеняем функцию, принимающую кортеж и id сотрудника
try: ... except ValueError: ... - Обработка исключения ValueError, которое возникает, если элемент не найден
start_index = log_tuple.index(employee_id) - Находим индекс первого вхождения элемента в кортеже
end_index = log_tuple.index(employee_id, start_index + 1): Находим индекс второго вхождения элемента, начиная с позиции после первого вхождения
return log_tuple[start_index:end_index + 1] - Возвращаем подстроку с первого появления элемента до второго включительно
return log_tuple[log_tuple.index(employee_id):] if employee_id in log_tuple else tuple() - Если элемент не найден, возвращаем пустой кортеж, если он встречается в кортеже

5.
Задача: объединить два списка в кортежи, которые состоят из элементов с одинаковыми индексами. Если списки разной длины, то кортежи формируются до конца более короткого списка.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/b9aaffe5-ecc4-4a0f-9a40-8d33ef39a9ae)
Вывод: def zip_lists(list1, list2) - Определяем функцию zip_lists, принимающую два списка.
min_length = min(len(list1), len(list2)) - Находим минимальную длину из двух списков, чтобы избежать ошибок при обращении к индексам
return tuple((list1[i], list2[i]) for i in range(min_length)) - Создаем кортеж из пар элементов с одинаковыми индексами из обоих списков. Используем генератор списка и функция tuple() для создания кортежа






































































