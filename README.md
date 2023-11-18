# Тема 7. Работа с файлами (ввод, вывод(
Отчёт по теме #7 выполнил:

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
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/021c327f-01da-4887-a493-6fab0e2db672)

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/e2e4f6b6-b2e7-4630-b492-97250ddfd05e)

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c5d1242c-9a97-444a-b991-1a4f652aa0bb)

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/44767ac6-cfe4-4b54-bf42-03bf62933476)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c534b7fc-661e-4cc7-bc49-df2e5b7865c1)

6.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/15b9e603-7096-407c-8834-49319b52580e)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/98fddc13-268f-455a-a4f4-d8d90998af68)

7.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2c13c2fb-bfdc-4ca8-bb53-84a9610b868f)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/2958ff27-94f5-4ec7-85c1-d6ff1d1149b2)

8.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c108080c-7f17-4900-922f-6d490ace6465)

9.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/5445b58a-75e8-4717-a279-dc053974fa22)

10.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/836e5848-e8b2-4333-bd85-1f04f1978bfb)

# Самостоятельная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/cf79933e-51be-418c-9632-6cb7e9bc1591)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/6e8a1ad1-5af7-4f92-8760-cb48f7ffffb0)
Вывод: Импортируем класс Counter из модуля collections и модуль re для работы с регулярными выражениями
Задаем путь к файлу, который нужно обработать
Открываем файл для чтения
Считываем содержимое файла, приводим его к нижнему регистру и находим все слова с использованием регулярного выражения
Подсчитываем общее количество слов в тексте
Используем Counter для подсчета частоты каждого слова и находим самое часто встречающееся слово и его количество в тексте
И выводим результаты

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/42f3c070-f5b4-4634-a510-8d74cd22022a)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/05a16d1d-549d-4132-96ac-5716faccddc5)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/1a4f8c99-d1b6-4262-a9d5-771b4805aded)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c7b5a3b2-3292-4e84-ac56-c5d8e3fa3717)
Вывод: Импортируем модули json и datetime
Определяем функцию input_expenses() для ввода расходов на товары
Определяем функцию save_expenses(), которая сохраняет введенные расходы в файл в формате JSON
В блоке if name == "main": запускаем основной цикл программы с опциями ввода расходов или выход
Печатаем опции в консоль
Запрашиваем у пользователя выбор действия (ввод расходов или выход)
Если выбран ввод расходов, вызываем функцию input_expenses() и сохраняем расходы с помощью функции save_expenses() и печатаем сообщение об успешном сохранении
Если выбран выход, завершаем программу
В другом случае, выводим сообщение о неверном вводе

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/9685046a-08d4-46dd-8523-c6647d3d4a86)
Вывод: Открываем файл и читаем его содержимое с использованием блока контекста
Подсчитываем количество букв в тексте
Подсчет количества слов в тексте
Подсчет количества строк в тексте
Возвращаем кортеж с результатами анализа
Потом попытка анализа текста в файле с указанным путем
Если файл найден, вывод результатов анализа (буквы, слова, строки)
Если файл не найден, вывод сообщения о том, что файл отсутствует

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/baf6ceb6-93b5-472c-ad09-e6e153e147dd)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/0415e353-baec-46a3-8a8b-ce9b0eab66c6)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/3f229838-9b26-4938-ba81-e45a7dd98c0b)
Вывод: создаем регулярное выражение для поиска запрещенных слов в любом месте предложения
Потом заменяем найденные запрещенные слова на звездочки
читаем запрещенные слова из файла input.txt
записываем предложение для проверки
далее заменяем запрещенные слова в предложении
и выводим результат
censor_sentence функция:
re.compile(r'(?:' + '|'.join(forbidden_words) + r')', flags=re.IGNORECASE) - создает регулярное выражение для поиска запрещенных слов в предложении без ограничения по границам слов
Флаг re.IGNORECASE делает поиск регистронезависимым
pattern.sub(lambda match: '*' * len(match.group(0)), sentence) - заменяет найденные запрещенные слова на звездочки, где количество звездочек равно количеству символов в слове

5.
Задание: написать программу на Python, которая считывает данные из файла и выводит список продуктов с ценами, превышающими 150 рублей,
а также посчитать общую стоимость всех продуктов в файле

![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/529b8334-24d9-47ba-bb0f-3c8215a21db8)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c7d23445-d0d5-4856-96cb-e8d633cb7b05)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/408cca90-5f12-4e7a-9cd2-0128fe96bd22)
Вывод: Создаем пустой словарь для хранения продуктов, цены которых превышают заданный порог
Преобразуем строку в число, заменяя запятую на точку
Добавляем продукт в словарь, если его цена выше заданного порога
Возвращаем словарь с отфильтрованными продуктами
Инициализируем переменную для хранения общей стоимости всех продуктов
Суммируем цены продуктов, преобразуя строки в числа
возвращаем общую стоимость всех продуктов
Выводим информацию о продуктах
Выводим общую стоимость 
