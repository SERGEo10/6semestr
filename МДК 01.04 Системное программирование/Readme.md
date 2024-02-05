# ЛК 15.01 gitbash - это команды для работы с гид из терминала bash создание репозитория на компьюторе: инициализация 1 $ git status On branch main указывает имя ветки No commits yet нет сохранений Untracked files: - неотслеживаемые файлы (use "git add ..." to include in what will be committed) - нужна команда добавить , чтобы зафиксировать версию index.html - список файлов для сохранения pictures/

nothing added to commit but untracked files present (use "git add" to track) - найдены файла для добавления Настраиваем ползователя в git git config --global user.name PK303-0 git config --global user.email PK303-0@gmail.com

git config --global --unset htpp.proxy git config --global --unset htpps.proxy git config --global --unset core.gitproxy 3 2 подтверждение 5 push основные ошибки:

remote - подключение к удаленном репозиторию (показывает на какой репозиторий мы хотим сохранить данные), может быть ошибка , что неправильно указали ссылку, чтобы изменить добавить set-url
авторизация - github нужно передать данные пользователя (логин,пароль или токин)
прокси сервер - проверям включен или нет лк 3 если есть папка .git то команду git init команда config настраиваются на пк (1 раз) git remote используется один раз
Пароли : qwerty - debian 12345678 - red os
