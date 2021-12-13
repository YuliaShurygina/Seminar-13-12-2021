# Инструкция по работе с Git

## Что такое Git?

Git - это одна из реализаций распределенных система контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой популярной системой контроля версий.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду git init в папке с репозиторием и у вас создастся репозиторий, появится скрытая папка .git.

## Создание коммитов

### git add

Для добавления файлов в репозиторий используется *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*.

### Просмотр состояния репозитория
Для того , чтобы посмотреть состояние репозитория применяем команду git status

### Создание коммитов
Для того,чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так *git commit -m"сообщение к коммиту"*. Сообщения к коммиту писать ***ОБЯЗАТЕЛЬНО***. 

## Перемещение между сохранениями

* Для того чтобы переместиться на какой-то из прошлых коммитов нужно использовать команду *git checkout*. Применяется она следующем образом в папке с репозиторием *git checkout <номер коммита>*. 

    **Пример** `PS D:\Юля\geek brains\Контроль версий\git_seminar> git checkout 750e`

* Для возврата к последнему коммиту ветки нужно использовать команду *git checkout master*.

    **Пример** `PS D:\Юля\geek brains\Контроль версий\git_seminar> git checkout master`

## Журнал изменений

Для просмотров истории коммитов используется команда *git log*. Для этого достаточно ее просто применить в папке с репозиторием.

Для каждого коммита есть свой идентификационный номер. Чтобы переходить от коммита к коммиту достаточно ввести 4 первые символа к команде checkout.

## Ветки в git

Ветка - это набор commit, которые идут друг за другом. У ветки есть название, основную ветку чаще всего называют master . Если говорить простыми словами, то ветка master - это наш проект.
Другие ветки - это отдельное место для реализации нового функционала или исправление багов (ошибок) нашего проекта. То есть, с отдельной веткой вы делаете что угодно, а затем сливаете эти изменения в основную ветку master.

Чтобы посмотреть сколько у нас на данный момент веток и какая из них текущая (в которой мы работаем) набираем команду *git branch*. Новые ветки создаем из ветки master. Для этого достаточно команду просто применить в папке с репозиторием. 

Чтобы создать новую ветку применяем команду *git branch < name>*.

Чтобы перейти от одной ветки к другой - *git checkout < name>*.

## Cлияние веток

Когда нас черновик полностью устраивает, мы можем перенести эту ветку в master.
Для того, чтобы перенести содержимое одной ветки в другую используем команду *git merge < branch name>*, здесь указываем имя переносимой ветки.  Команду выполняем из той ветки, в которую нужно перенести наш черновик. 

## Удаление веток

Если ветка - черновик больше не нужна, то можем ее удалить. 
Для того, чтобы удалить ветку нужно выполнить команду  *git branch -d < branch name>*. 

