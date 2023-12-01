# Тема 9. Концепции и принципы ООП
Отчёт по теме #9 выполнил:

• Непеин Никита Сергеевич

• ПИЭ-21-1
| Задание | Лаб_раб | Сам_раб |
| --- | --- | --- |
| Задание 1 | + | + |
| Задание 2 | + |  |
| Задание 3 | + |  |
| Задание 4 | + |  |
| Задание 5 | + |  |

# Лабораторная работа

1.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/a290472b-6197-4df3-a6d6-0e0c01657103)

2.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/cfa31f57-73d5-4021-bde6-5df9fd74ac61)

3.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/626d8173-605e-45da-82ed-48a1a30688b3)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/d88e031c-9135-49ab-ac6e-fae6b684b2f6)

4.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/493914d5-b740-490f-a088-880fcf314962)

5.
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/5b86abb7-836b-4984-bd5b-4904033bbb45)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c414bd87-2036-470f-92ad-750e9c8a3fa5)

# Самостоятельная работа

![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/65dae83a-a606-4c3a-93ef-e6343accce62)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/c2b97b55-ef91-46bf-bf6b-f735a9e0be63)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/7114f9f3-0fec-4c8b-a587-70ba88b6ed03)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/fd2e97ad-2414-417a-806e-5ac4181988c9)
![image](https://github.com/yarcheee/Software_Engineering/assets/99402010/0bf94664-13ec-403a-b79f-abc92241417f)

Вывод:
1)	Вызвал справку по руководству с помощью метода knowledge_base
2)	Создал объекты классов TomatoBush и Gardener
3)	Используя объект класса Gardener, ухаживал за кустом
4)	Попробовал собрать урожай, когда томат ещё не дозрел и выводит - "Томаты еще не дозрели. Продолжайте ухаживать за ними."
5)	Собрал урожай


# Tomato класс, представляющий помидор
class Tomato:
    
    # Статическое свойство с состояниями зрелости помидора
    states = {
        0: "Отсутствует",
        1: "Цветение",
        2: "Зеленый",
        3: "Красный"
    }

    # Инициализация экземпляра класса Tomato
    def __init__(self, index):
        self._index = index
        self._state = 0

    # Метод для перевода помидора на следующую стадию зрелости
    def grow(self):
        if self._state < len(self.states) - 1:
            self._state += 1

    # Метод для проверки, созрел ли помидор
    def is_ripe(self):
        return self._state == len(self.states) - 1


# TomatoBush класс, представляющий куст помидоров
class TomatoBush:
    # Инициализация экземпляра класса TomatoBush
    def __init__(self, num_tomatoes):
        # Создание списка помидоров с указанным количеством
        self.tomatoes = [Tomato(i) for i in range(1, num_tomatoes + 1)]

    # Метод для перевода всех помидоров куста на следующую стадию зрелости
    def grow_all(self):
        for tomato in self.tomatoes:
            tomato.grow()

    # Метод для проверки, все ли помидоры созрели
    def all_are_ripe(self):
        return all(tomato.is_ripe() for tomato in self.tomatoes)

    # Метод для сбора урожая и очистки списка помидоров
    def give_away_all(self):
        self.tomatoes = []


# Gardener класс, представляющий садовника
class Gardener:
    
    # Инициализация экземпляра класса Gardener
    def __init__(self, name, plant):
        self.name = name
        # Привязка садовника к растению
        self._plant = plant

    # Метод для ухода за растением (перевода его на следующую стадию зрелости)
    def work(self):
        self._plant.grow_all()

    # Метод для сбора урожая
    def harvest(self):
        if self._plant.all_are_ripe():
            # Вывод сообщения о сборе урожая и очистке списка помидоров
            print(f"{self.name} собрал урожай!")
            self._plant.give_away_all()
        else:
            # Вывод предупреждения, если не все помидоры созрели
            print("Томаты еще не дозрели. Продолжайте ухаживать за ними.")

    # Статический метод справки по садоводству
    @staticmethod
    def knowledge_base():
        print("Справка по садоводству:")
        print("- Работайте с растением, вызывая метод work().")
        print("- Проверяйте зрелость плодов вызовом метода harvest().")
        print("- Если все плоды созрели, соберите урожай вызовом метода harvest().")


# Тесты
# Вывод справки по садоводству
Gardener.knowledge_base()
# Создание куста с 3 помидорами
bush = TomatoBush(3)
# Создание садовника по имени Никита
gardener = Gardener("Никита", bush)

print("\n--- Первый цикл ухода и проверка урожая ---")
gardener.work()
gardener.harvest()

print("\n--- Продолжение ухода ---")
gardener.work()

print("\n--- Завершение ухода и сбор урожая ---")
gardener.work()
gardener.harvest()






















