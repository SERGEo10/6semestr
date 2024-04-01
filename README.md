# 6semestr

Задание 11. Измерение времени и чтение из базы данных 
Разработать программу, которая будет принимать дату, длительность и список переменных и измерять длительность операции чтения указанной группы переменных из таймсериез базы данных.
1. Создаем папку dbselect
2. В файле __main__.py мы используем библиотеку argparse для обработки аргументов командной строки.
Argparse позволяет конвертировать строковые аргументов в объекты нашей программы и работать с ними; выводит информативные подсказки.

import argparse
from datetime import datetime
import time  # Будем использовать для имитации чтения из базы данных и измерения времени

def main(date, duration, variables):
    start_time = time.time()
    # Здесь будет ваш код для чтения из базы данных. Сейчас просто имитируем задержку.
    time.sleep(2)  # Имитация задержки чтения данных, например, 2 секунды
    print(f"Чтение переменных {variables} за {time.time() - start_time} секунд.")

if __name__ == "__main__":
    parser = argparse.ArgumentParser(description="Измерение времени операции чтения из базы данных.")
    parser.add_argument("date", type=lambda s: datetime.strptime(s, '%Y-%m-%d'), help="Дата в формате YYYY-MM-DD")
    parser.add_argument("duration", type=int, help="Длительность в секундах")
    parser.add_argument("variables", nargs='+', help="Список переменных для чтения")

    args = parser.parse_args()

    main(args.date, args.duration, args.variables)
