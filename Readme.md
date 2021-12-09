# Инструкция по работе с Git

## Что такое Git?

Git - это одна из реализаций распределенных система контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой популярной системой контроля версий.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду git init в папке с репозиторием и у вас создастся репозиторий, появится скрытая папка .git.

## Создание коммитов

### git add

Для добавления файлов в репозиторий используется *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*.


### Создание коммитов
Для того,чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так *git commit -m"сообщение к коммиту"*. Сообщения к коммиту писать ***ОБЯЗАТЕЛЬНО***. 

## Перемещение между сохранениями

* Для возврата к последнему коммиту ветки нужно использовать команду *git checkout master*.

    **Пример** `PS D:\Юля\geek brains\Контроль версий\git_seminar> git checkout master`


## Журнал изменений

Для просмотров истории коммитов используется команда *git log*. Для этого достаточно ее просто применить в папке с репозиторием. 

## Ветки в git

## Cлияние веток

## Удаление веток