# ЛК1 15.01.24.

Git Bash - команды для работы с Git из терминала 

[Установка Git Bash](https://git-scm.com/downloads)

Прокси сервер git config --global http.proxy 10.0.50.52:3128

[Практические работы](https://smartiqa.ru/courses/git/answer-key)

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/44710bc2-9235-413e-94f3-8fda8c24a6bf)

Создание репозитория на компьютере: Инициализация Git Init

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/25d26c97-b57a-4a52-99a4-cad392da6bd7)

cmd //c tree .git - показывает структуру папки git

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/819f0ec2-b451-4ec9-acde-366de8262709)

git status - Показывает статус репозитория On branch master - Указывает имя версии

No commits yet - Нет сохраненных версий

Untracked files: - Неотслеживаемые файлы

(use "git add ..." to include in what will be committed) - Нужна команда добавить, чтобы зафиксировать версию для сохранения

    index.html
    pictures 
список файлов для сохранения

nothing added to commit but untracked files present (use "git add" to track) - Найдены файлы для добавления


**Задаем имя и email пользователя для текущего репозитория 23-12 303-15**
 
$ git config  --global user.name PK303-12 

$ git config  --global user.email PK303-12@gmail.com


**Отменяют прокси**

$ git config --global –unset http.proxy

$ git config --global --unset https.proxy

$ git config --global --unset core.gitproxy

Добавление файлов - git add * 

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/5e2aa216-dead-45b3-8ce1-0203cde9ff14)

**Для фиксации версии нужно указаь ее название, для этого создается сообщение** 
$ git commit -m "G-02: Initial"

**Выводим информацию о фиксации** 
$ git logl"

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/f1146ee2-bd13-49f3-ad2a-697ec8363ded)

**Подтверждение git**

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/9284ce83-fff5-4fd3-902e-6b0a049d0db8)

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/5516acef-cf5d-44c7-9649-2f3000b79913)




![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/a891cce3-5cc1-4eb7-ac85-4ab5fa9ccb41)

Основные ошибки :

1. Remote - подключение к удаленному репозиторию (показывает на какой репозиторий мы хотим сохранить данные), может быть ошибка что неправильно укзали ссылку. Что бы изменить -> добавить сейт-URL
2. Авторизация - гитхабу нужно передать данные пользователя (логин, пароль или токен)
3. Прокси сервер - проверять включен или нет


# ЛК2 22.01.24.

1. Если есть папка _.git_, то команду _git init_ выполнять не нужно
2. Команды _config_ настраиваются на ПК 1 раз
3. _git remote_ указывается 1 раз

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/1190e164-00df-44c4-976b-c1d93667afb3)

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/5f3e4844-f4eb-4e1f-8f66-c927c8870f2a)

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/0869ec52-ce89-458f-9c6b-3bc948ccfa35)


**Дебианс**

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/3e2326b1-3229-4dad-ad5f-e35ca17dea4d)

![image](https://github.com/b6e6b6r6a/6_Semestr-/assets/113089548/0c84387a-5eac-45e1-87ef-9a8c873504ae)

**РедОС python**

![image](https://github.com/SERGEo10/6semestr/assets/106819250/1b97a25c-3f3d-4535-9e67-9a233fb20296)


# ЛК3 05.02.24.

1. Создание 
2. Перемещение
3. Редактирование
4. Удаление 

Обычный файл (Regular file)

1. touch ccl.txt
2. mv ccl.txt /home/stud/'Рабочий стол'
3. nano /home/stud/'Рабочий стол'/ccl.txt; cat /home/stud/'Рабочий стол'/ccl.txt

![image](https://github.com/SERGEo10/6semestr/assets/106819250/ad70dbcc-248c-4b42-9a5d-7170ea8e420e)

Для RedOS

![image](https://github.com/SERGEo10/6semestr/assets/106819250/3a66f34a-c68d-4770-a470-758f91d3fb5a)


Папка (Directory)

1. mkdir ccl
2. touch /home/stud/ccl/xxl.txt
3. ls /home/stud/ccl

![image](https://github.com/SERGEo10/6semestr/assets/106819250/302039c3-6ac6-42b2-8f3f-88d73b9f852d)

Для RedOS 

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b76128b1-8dd2-42a9-830b-96787cfb3d22)

**Жёсткие и символьные ссылки**

ln -s main.txt smain.txt - мягкая ссылка ln main.txt hmain.txt

![image](https://github.com/SERGEo10/6semestr/assets/106819250/27b68833-f476-4946-bfe8-53cc0597dea6)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/d2e58626-9c87-4cbc-b682-79178f1f78bd)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/89513f02-e158-4ef9-bc1b-8f362e6e9637)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/8d215f50-3e2b-4566-abf5-560bba75369b)



**Передача данных: сокет(socket) и каналы(pipe)**

Разница в способе передачи данных

Fifo - first in first out 

![image](https://github.com/SERGEo10/6semestr/assets/106819250/e53fcba1-5d3c-4d12-99a9-ab27e792394c)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/51084aaa-e7e6-4a29-b605-56f6337a306c)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/1f21d9cf-dd74-425b-8a55-476d3e67628b)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b3ac4845-df47-4b1f-b1e6-d9635d689064)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b4b53825-abb9-45bf-9afa-21bb06503e8d)



# 12.02.24
Устройство:
1. Символьные(мышь, клавиатура)
2. Блочные(флешки)

mknod
mknod blockf b 5 100
nano blockf
rm blockf

![image](https://github.com/SERGEo10/6semestr/assets/106819250/22b07200-d0f3-4e39-a434-8258084046e7)

mknod charf c 5 100

![image](https://github.com/SERGEo10/6semestr/assets/106819250/ea5a46b6-a292-41bb-a6ee-e2f90267dc65)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/6e8256d3-2bae-4855-af7e-960c1e0a4f37)

Файлам присваивается уникальный номер - enod, посмотреть командой ls i1. Жёсткие ссылки имеют тот же номер, что и исходный файл и это можно использовать чтобы найти все жёсткие ссылки.

**Скрипты**

![image](https://github.com/SERGEo10/6semestr/assets/106819250/d8199296-0d5d-4c76-821e-7b9852fbe802)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/18e6046d-fffb-474d-922a-5c3e65ea1e20)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/ec873e9a-2335-47ef-bd16-29b374ff4773)

# ЛК 3 19.02 Пользователи

![image](https://github.com/SERGEo10/6semestr/assets/106819250/f33313ef-5de9-4e96-96d4-1390664133f3)

stud - имя пользователя x - пароль 1000 - номер пользователья 1000 - номер группы

bin\bash - терминал пользователя

![image](https://github.com/SERGEo10/6semestr/assets/106819250/a7aaede6-d14c-4213-966f-a0c7adb58d3d)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/8b2711a4-b44d-4778-81b9-f080b04e0bea)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/22eeba89-5e98-4d25-a06b-17464039147e)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/c77843a3-6470-4dc9-a226-188a185b7f45)

**Дебиан**

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b45e6b9c-f456-44af-9e53-a4c0d88a2992)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/7fef3c95-ef8c-4176-9ec1-62d93775a6bb)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/574a560a-b49a-4d80-acfe-67ce6fb7d48a)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/2ecd2b8e-d321-4bfc-b284-99de8824328a)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/20a9e29d-e445-4bed-bd5d-1930cbe885c7)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/0133fda4-ccb0-44d9-8556-68d1ca483d52)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/4ec28e79-c3af-455d-81a2-9f9b55b18309)


**РедОС**

![image](https://github.com/SERGEo10/6semestr/assets/106819250/9ee3bde0-ee99-4caa-be68-32d212ca486a)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/099e0303-f979-455b-b21c-2a4fa81fabe6)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/8a924ace-541d-4909-a1fb-c93c23ca4d49)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/75a46689-b8bf-4c1a-9b5b-064175bbcd1e)
![image](https://github.com/SERGEo10/6semestr/assets/106819250/b3560842-bb76-4312-a13e-20efc42dbd83)

# ЛК 4 04.03 Структура памяти процесса

**Debian**

![image](https://github.com/SERGEo10/6semestr/assets/106819250/9421f30f-8dca-404c-98a4-f30610577bfb)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/4ad56eb8-6d9c-42e3-980e-e8c651f757e6)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/ae1222b8-f641-46e6-922e-1fb97f98e82d)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/ae99b8bb-2807-401d-9888-324654512d49)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/cd94ad76-b270-4ef7-8ced-cd0ce96d6b5b)

Переполнение стэк

![image](https://github.com/SERGEo10/6semestr/assets/106819250/1f11ee4b-212d-4a2e-b2a3-38477d3bbcdf)


**RedOS**

Вывод процессов

![image](https://github.com/SERGEo10/6semestr/assets/106819250/c417d9be-4560-4a8e-abf9-179c8b750060)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/00b3bc25-39fb-497b-8bf1-c40b7497e365)

Запуск программы, код программы

![image](https://github.com/SERGEo10/6semestr/assets/106819250/455c9ad9-5c95-4907-ae8c-2d2d47b84792)

Код программы

![image](https://github.com/SERGEo10/6semestr/assets/106819250/559d5dcb-9c54-454b-8c88-4a7419acbcab)

Переполнение стек

![image](https://github.com/SERGEo10/6semestr/assets/106819250/af649346-db98-4c7d-aa28-633ce3f4d543)

# ЛК 5 11.03 Потоки в БД

Аттрибуты процесса:
1. PID - уникальный идентификатор 
2. Адресация областей памяти
3. FD - открытые файловые дескрипторы(терминал или файлы которые используют процессы)
4. Обработчики сигналов процесса(запросы от пользователей)
5. Код выходы(ctrl+c, ctrl+z, all done, exit button)
6. Рабочий каталог(версия ОС)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/8279c990-bef1-4b8b-96ac-a9f401495151)

Первый процесс в системе это init

![image](https://github.com/SERGEo10/6semestr/assets/106819250/3b847e60-7333-4a8e-a4a7-3dbdd07c41d6)

Смерть процесса - exit() или kill, завершение процесса:
1. Остановка дочернего процесса - либо переподключится, либо станет зомби
2. Завершили родительский - либо дочерний будет зомби, либо подключиться к другому родительскому
3. Ready - процесс готов в выполнению, но находится в очереди
4. Running - это запущен(ctrl+c - stop, ctrl+z - сон)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b61d1df1-ab06-4223-82ca-64292dc1677b)

**Сигналы**

Сигнал - это способ оповестить процесс о наступлении события.

![image](https://github.com/SERGEo10/6semestr/assets/106819250/b9d9e70e-7a23-44f0-8142-e5f033cd9735)

**Прервывания**

Аппаратные и программные. К аппаратным относиться клавиатура, мышка и т.д. К программным всё что с кодом и т.д.

**Планировщик процессов**

Вытесняющая и кооперативная многозадачность. Кооперативная - программа сама решает когда нужно прекратить выполнение. Вытесняющая решение о переключение на другой процесс принимает сам планировщик.

**Синхронизация процессов в ОС** 

Это управление тем, чтобы несколько программ могли работать вместе, не мешая друг другу, особенно когда они используют одни и те же ресурсы.

**Мьютексы**

Это инструменты, позволяющие только одной программе в один момент времени использовать общий ресурс, чтобы избежать конфликтов.

**Семафоры**

Это похожие на мьютексы инструменты, которые могут управлять доступом к ресурсам нескольким программам одновременно, но более гибкие, чем мьютексы.

**Критические секции** 

Это части программного кода, которые защищаются от одновременного доступа нескольких программ, чтобы избежать проблем с данными.

**Файловые блокировки**

Это способ защитить файлы от одновременных изменений несколькими программами, чтобы избежать потери или повреждения данных.

**Debian**

Подключение к БД

![image](https://github.com/SERGEo10/6semestr/assets/106819250/94d68e1e-b4bd-4aaf-9503-fd232a5cdc3c)

Запуск и проверка состояния сервера

![image](https://github.com/SERGEo10/6semestr/assets/106819250/e343add7-b362-4cb6-80a2-2659cc98e9bd)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/0cde8502-8ea8-4c4b-9ff2-549a1d9e94c8)

Переход в работу с базой данных

![image](https://github.com/SERGEo10/6semestr/assets/106819250/0108cb98-041b-4c9d-ab82-53fa17f7aff3)

Создание и изменение данных в таблице

![image](https://github.com/SERGEo10/6semestr/assets/106819250/c9ea98d8-87c1-4832-87ec-990baa3da964)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/e5cac84f-9d98-42bf-af5f-b649cfb269c8)

Структура БД

![image](https://github.com/SERGEo10/6semestr/assets/106819250/5f3613e6-25af-47ca-a5ec-8ed497d27796)

Проверяем количество строк

![image](https://github.com/SERGEo10/6semestr/assets/106819250/1e659467-99fb-4258-baa8-36f9cb6e087b)

Далее создадим класс Cursor, при инициализации которого вызывается блокировка потока, обнуляется позиция и передается количество строк в базе. Для потоко-безопасного получения следующего индекса напишем функцию next, которая смещает счетчик позиции на 1, пока мы не пройдем по всем строкам базы. Чтобы пользователь видел, на каком шаге программа, будем выводить в консоль на какой мы позицию с шагом в 10.000. Пример вывода на экран на скриншоте:

![image](https://github.com/SERGEo10/6semestr/assets/106819250/fc2e593e-507e-4dd2-8859-63c058ca7d12)

Подключаемся для каждого потока к нашей БД, определяем нашу позицию с помощью класса Cursor и создадим файл для записи с именем res_Номер потока_False, где False означает, что вначале рассматривается использование буфера.

![image](https://github.com/SERGEo10/6semestr/assets/106819250/a0375673-7b9b-4669-9158-ea3a0e590e67)

Когда мы не используем буфер, строки сначала записываются во все 10 файлов, потом 11 снова записывается в первый файл. Функция flush очищает выходной буфер и перемещает буферизованные данные на диск. Мы создали условие if flush: (чтобы использовать ее только во 2м случае, когда передадим параметр True). В этом случае сначала все строки записываются в 0-й файл, потом переходят к 1-му и так далее. Flush — Сброс системного буфера вывода.

![image](https://github.com/SERGEo10/6semestr/assets/106819250/3241d4bf-8634-4e75-acbd-a9726c91c417)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/13f6ce5e-c4db-4ea6-8457-2454b00c4ed2)

![image](https://github.com/SERGEo10/6semestr/assets/106819250/93b25ba3-8f0c-4c71-84f8-e2ffa9399536)

# ЛК 6. Брокеры сообщений и докер

RabbitMQ - брокер сообщений с открытым исходным кодом. Брокер - инструмент для передачи данных

![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/c6098d6b-7048-4bd1-b11f-33a4deb876ae)

У нас есть издатель и потребитель. Сообщения хранятся в очереди(queues). Обмен(Exchange) и распределение между очередями(binding).
Docker - ПО с открытым кодом, позволяет переносить программные продукты. Может съедать много памяти.

![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/d3cbf4ca-e09c-49cb-89fc-4a624ef9d116)

Клиент - интерфейс. Демон - управление объектами докера. Контейнер - программа. Образ - конфигурация в файле.

**Задание 6**

![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/92006ac0-3b19-4fe1-94c6-3af33bad982f)
![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/2a211e36-21a0-4c42-959a-477906b3b79f)
![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/e396ad4c-7a0e-4555-a042-da59cb6ecf82)

![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/6981886b-6dce-4f1d-a119-b0b0322b8008)


![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/ec4bcb03-a291-461b-b1a5-849e68a20cff)
![image](https://github.com/zdarova69/USMONOVNN-IS21/assets/113101818/85507324-8bfe-4624-8aac-3f28b4f7efcd)



















