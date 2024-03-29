https://docs.google.com/document/d/10qMdyxy1n7iskraPvv3sO8xSzCysdejjeM9nsxgLSd8/edit - Postman.

# ЛК 2 12.02 TDD

TDD - разработка через тестирование. 

Жизненный цикл ПО:
1. Каскадная модель
2. V-модель
3. Итеративная или инкрементальная модель
4. Спиральная модель.

У каскадной модели:
1. Под тестирование выделен только один этап. Дефекты во время эскплуатации нельзя исправить.
2. Нет плана тестирования

У V-модели тестируется каждый этап.

У итеративной и инкрементальной:
1. Большие объёмы регрессионного тестирования 
2. Отсутствие плана.

У спиральной системы:
1. Сложно тестировать на ранних этапах, но тестирование становится ключевым этапом.

![image](https://github.com/SERGEo10/6semestr/assets/106819250/50391609-e7ec-43b5-bb7f-76443445c355)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/832fa3cf-0433-4fdc-b0df-12cc6488966c)

Уровень тестирование:
1. Компонентное
2. Интреграционное
3. Системное
4. Приёмочное

Тестирование бывает статическое и динамическое. Статическое без исполнения кода, динамическое с исполнением кода.
![image](https://github.com/SERGEo10/6semestr/assets/106819250/bf355d88-c302-4a14-a77f-8fd64e750cb4)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/7ccfe14b-bd52-421d-9468-8e592e77e084)

Различные виды тестирования.

Функциональные тесты:
1. Загрузка торрент файла
2. Раздача скорости после скачивания файла
3. Возможность ставить и возобновлять скачивание файла.

Тесты производительности:
1. Скорость скачивания торрент файла
2. Скорость раздачи торрент файла
3. Лимиты приёма и отдачи файла.

Нагрузочные тесты:
1. Загрузка двух торрент файлов одновременно
2. Раздача разных торрент файлов одновременно.

Тестирование совместимости:
1. Наличие совместимости с Linux системами.

Различные типы тестов.

Позитивные тесты:
1. Файл скачался с нормальной скоростью
2. Файл раздавался в течении длительного периода без сбоев.

Негативные тесты:
1. Пользователь без премиума будет видеть рекламу
2. Без подключения к интернету, не будет возможности скачать файл.

Исследовательские тесты:
1. Торрент файл может быть назван кириллицей.

Различные области тестирования.

Модульное тестирование:
1. Установка в пути указаном при скачанивании торрента
2. Установка ограничения по скорости скачивания торрент файла.

Интеграционное тестирование:
1. Возможность работы с базой данных
2. Правильно ли работают модули показа статистики по скачиванию файла.

Системное тестирование:
1. Основной смысл приложения выполняет свои обязанности по скачиванию файла
2. Встроенное видео проигрывается, скорость скачивания файла отображается корректно.

# ЛК 3 19.02 Дефекты

Отчёт о дефекте - это документ, который содержит информацию о том, что может привести систему к невозможности выполнить требуемую функцию.
![image](https://github.com/SERGEo10/6semestr/assets/106819250/d4d30629-058a-458e-a2de-229dab803738)

Отчёт о дефекте включает:
1. Идентификатор
2. Краткое описание: Характер проблемы, границы дефекта, последствие дефекта.
3. Подробное описание: ожидаемый и фактические результаты
4. Влияние: критичность и приоритет

Причины почему дефекты не устраняют
1. Не хватка времени
2. Дефект вовсе не дефект(фича)
3. Устранение неисправности слишком рискованно
4. Это того не стоит
5. Неэффективный отсчёт

![image](https://github.com/SERGEo10/6semestr/assets/106819250/8337b76f-ec45-45ca-bd69-311902f3711b)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/64b64594-7850-4d63-b451-790858d6e1d9)

**Заголовок:**
Неверные результаты сложения в калькуляторе Windows

**Описание:**
При проведении тестирования калькулятора Windows были обнаружены некорректные результаты операций сложения. Данный дефект приводит к тому, что некоторые выражения вычисляются неверно.

**Шаги воспроизведения:**
1. Открыть калькулятор Windows.
2. Выбрать режим "Обычный" или "Научный".
3. Ввести следующие выражения и нажать кнопку "Равно".
 
**Ожидаемый результат:**
1. 1 + 1 = 2
2. 2 + 2 = 4
3. 3 + 3 = 6
4. 4 + 4 = 8
5. 5 + 5 = 10
6. 6 + 6 = 12

**Наблюдаемый результат:**
1. 1 + 1 = 2 (Ожидаемый)
2. 2 + 2 = 5 (Неверный)
3. 3 + 3 = 6 (Ожидаемый)
4. 4 + 4 = 9 (Неверный)
5. 5 + 5 = 10 (Ожидаемый)
6. 6 + 6 = 13 (Неверный)

**Влияние:**

Данная проблема может оказать критическое влияние.

**Тестовый сценарий**

Тестовый набор: 
1. Тестовые сценарий 
2. Тестовые данные
3. Или правило генерации тестовых данных

Выбор данных:
1. Покрытие операторов
2. Покрытие узлов ветвления
3. Комбинаторное покрытие условий

**Классы эквивалентности** - Одинаковая верояность обнаружения конкретного типа обнаружения

![image](https://github.com/SERGEo10/6semestr/assets/106819250/9c0ecc60-8369-4020-a004-ebd4b5c82798)

https://docs.google.com/document/d/11lv4z1qVRJYPmHen8uuUZ7msKK9WPY6wfhnwr5KKWQc/edit?usp=sharing

# Лекция 4. Unit test

unit тест - функция, которая проверяет 1 действие из кода. Есть ожидаемый результат - если ожидаемый результат не получен - тест не пройден.

Наименовение проектов:
На дем экзамене могут снять баллы, если даны названия функций, а вы их не использовали.

Arrange-Act-Assert

Arrange - предусловие 
Act - действие
Assert - постусловие 

![image](https://github.com/SERGEo10/6semestr/assets/106819250/3b30b5cb-a76e-4d8a-bfef-846bb38f9748)

1. Тестирующий класс - это имя файлов и класс обычно под имя файла обычно переименовывается 
2. Тестирующий метод - это функция которую нужно протестировать
 
![image](https://github.com/SERGEo10/6semestr/assets/106819250/861347d7-adbb-4e8a-ba4b-96884a4be0ed)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b4a906b5-764f-453d-b402-28da1a58cffd)

Нужно 2 файла. 1 файл программа которую нужно протестировать, а 2-ой сами тесты. 

ПКМ по имени функции

![image](https://github.com/SERGEo10/6semestr/assets/106819250/4ab2bdb4-049b-4d7b-aead-f25dfe2448bd)

Простой вариант

![image](https://github.com/SERGEo10/6semestr/assets/106819250/2c246489-8d5c-4714-88cd-2d04e7624a43)

Сложный вариант

![image](https://github.com/SERGEo10/6semestr/assets/106819250/c0b93c02-4423-4d01-9e03-8c0cad22aa07)

Файл собранной библиотеки имеет расширение dll и страницу bin debug

![image](https://github.com/SERGEo10/6semestr/assets/106819250/9e770029-ad17-426c-adc9-c5a38d3dafec)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/dcd77330-9c1f-4a7c-ac5e-42d595e5f509)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/246d1928-4a02-4adc-aea5-2446f5b27ac8)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/4e9d190e-4771-4af2-b8ee-e6c6caf3b6a7)




