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



























