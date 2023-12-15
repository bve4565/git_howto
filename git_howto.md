# Подсказка по GIT

Создание репозитория:
```sh
git init
```

Добавление отслеживания файла
```sh
git add <filename>
```

Добавление фиксации файла
```sh
git commit -m "Message text"
```

Просмотр лога
```sh
git log
```

Вывод сокращенных комитов
```sh
git log --oneline
```

Перемещение по веткам
```sh
git checkout <имя_ветки>
```

Отображение всех веток 
```sh
git branch
```

Создание новой ветки
```sh
git branch <branch_name>
```

Команда удаления ветки
```sh
git branch -d <name_branch>
```

Посмотреть лог в сокращенном графическом виде
```sh
git log --oneline --graph
```
# Это репозиторий для обучения pull request

## Первые шаги

1. Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку Fork на странице репозитория <https://git@github.com:gulden-geekbrains/version_control.git>
2. Выполняем команду клонирования из своей fork-копии
```sh
git clone git@github.com:*YOURE_GITHUB*/version_control.git
```
3. Создаем новую ветку и вносим необходимые изменения в файл
```sh
git checkout -b updatereadme
vim README.md
git add README.md
git commit -m "Добавили инструкцию как создать pull request"
```
4. Делаем push  
```sh
git push --set-upstream origin updatereadme
```
5. Переходим на свою страницу репозитория. Выбираем ветку **updatereadme** и жмем кнопку **Compare & pull request**

## Заметки

Что бы сделать push от другого пользователя необходимо выполнить команду
```sh
GIT_SSH_COMMAND='ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes' git push git@github.com:gulden-geekbrains/version_control.git
```

вместо *user-private-key* подставьте свой ключ

Можно прописать настройки для подсоединения по ssh
```sh
git config remote.origin.url git@github.com:gitusername/reponame
git config core.sshCommand "ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes"
```
# Как подружить git с github под Windows 10

Вот видео инструкция https://youtu.be/E8cIjbJMEpE
