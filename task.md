Дополнить файл с инструкцией по работе с git (второе домашнее задание) и направить pull request в этот репозиторий. Файл с инструкцией необходимо дополнить информацией о работе с удаленными репозиториями.

 Инструкция по работе с git репозиторием
## Для начала работы:
> git unit

R
если имя пользователя т почта ещё не были заданы:
> git congig --global user.name

> git congig --global user.mail

## Работа с файлами:
Для того, чтобы добавить файл, нужно:
1. git add file_name

    добавляем файл с именем file_name для отслеживания
2. git commit -m "some message"

    добавляем текущие изменения в репозиторий и подписываем их с помощью тега -m

Чтобы отслеживать состояние репозитория:
1. > git status
2. > git log
3. > git diff

чтобы показать ветки:
> git log --graph



## Работа с коммитами
Для того, чтобы перейти к определенному комиту, можно использовать команду
git checkout code_commit
    code_commit - код коммита, к которому мы хотим перейти, его можно просмотреть в git log

Чтобы вернуться к самому последнему состоянию: 

git checkout master

![flowers](original.jpeg)

## Ветки в git 
Чтобы посмотреть все ветки:
> git branch

Для создания ветки с именем branch_name:
> git branch branch_name

Переместиться к ветке с именем branch_name:
> git checkout branch_name

## Слияние веток и решение конфликтов
Чтобы слить информацию из ветки branch_name в текущую:
> git merge branch_name

В случае конфликта нужно удалить все лишние строки и оставить ту часть, которая нужна. Если необходимо, то можно отредактировать её.

## Удаление веток
Для того, чтобы удалить ветку с именем branch_name:
> git branch -d branch_name

Удаление с игнорированием ошибок: 
> git branch -D branch_name

Примеры применения тега:
