# **Инструкция для работы с git**

## Что такое git

__git__ - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Эта инструкция показывает команды необходимые для начала работы в __git__.

## Подготовка к работе 

Перед работой в git необходимо прредоставить свои данные, представиться. 

Что бы выполнить это условие необходимо в командную строку git ввести следующие команды:
* **git config --global user.name** "<*ваше имя пользователя*>"
* **git config --global user.email** "<*ваш адрес электронной почты*>"

После этих действий можно приступать к работе в git.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду:
* **git init** - в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

Для проверки статуса файла и его состояния введите следующую команду:
* **git status** - если файл отслеживается его цвет будет $ \color {green} {зеленым} $, если же нет $ \color {red} {красным} $ 

## Создание коммитов
Для создания коммитов(схранений), вам потребуются следующие команды:
* **git add** <*имя файла*> - комада используестя для того что бы git понял с каким файлом  мы работаем, добавляем файл для дальнейшего коммита.
* **git commit -m** "<*сообщение к коммиту*>" - команда создает коммит, все файлы для коммита должны быть __ДОБАВЛЕНЫ__ и сообщение к коммиту писать __ОБЯЗАТЕЛЬНО__.

## Поиск и перемещение между коммитами

Для перемещения между ветками потребуются следующие команды:

* **git log** - команда показывает список коммитов и их номера.
* **git checkout** <*номер коммита или название ветки*> - команда позвоняет перемещаться между коммитами и ветками.
* **git diff** - команда показывает разницу между текущим коммитом и предыдущим. 

# Создание веток в git
* **git branch** <*название новой ветки*> - команда создает новую ветку, для работы в новой ветке необходимо использовать команду checkout.
* **git merge** <*название ветки*> - команда добавляет в текущую ветку, ветку которую вы указали в названии ветки.
* **git branch -d** <*название ветки*> - команда удаляет не нужную ветку, обычно ветки удаляют после их слияния с веткой master.