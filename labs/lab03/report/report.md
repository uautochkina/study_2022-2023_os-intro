---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: 
author: "Уточкина Ульяна Андреевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

    Изучить идеологию и применение средств контроля версий.
    Освоить умения по работе с git.

# Теоретическое введение

Основные команды git

    Перечислим наиболее часто используемые команды git.

    Создание основного дерева репозитория:

    git init

    Получение обновлений (изменений) текущего дерева из центрального репозитория:

    git pull

    Отправка всех произведённых изменений локального дерева в центральный репозиторий:

    git push

    Просмотр списка изменённых файлов в текущей директории:

    git status

    Просмотр текущих изменений:

    git diff

    Сохранение текущих изменений:

        добавить все изменённые и/или созданные файлы и/или каталоги:

        git add .

        добавить конкретные изменённые и/или созданные файлы и/или каталоги:

        git add имена_файлов

        удалить файл и/или каталог из индекса репозитория (при этом файл и/или каталог остаётся в локальной директории):

        git rm имена_файлов

    Сохранение добавленных изменений:

        сохранить все добавленные изменения и все изменённые файлы:

        git commit -am 'Описание коммита'

        сохранить добавленные изменения с внесением комментария через встроенный редактор:

        git commit

        создание новой ветки, базирующейся на текущей:

        git checkout -b имя_ветки

        переключение на некоторую ветку:

        git checkout имя_ветки

            (при переключении на ветку, которой ещё нет в локальном репозитории, она будет создана и связана с удалённой)

        отправка изменений конкретной ветки в центральный репозиторий:

        git push origin имя_ветки

        слияние ветки с текущим деревом:

        git merge --no-ff имя_ветки

    Удаление ветки:

        удаление локальной уже слитой с основным деревом ветки:

        git branch -d имя_ветки
        принудительное удаление локальной ветки:

git branch -D имя_ветки

удаление ветки с центрального репозитория:

git push origin :имя_ветки


# Выполнение лабораторной работы
 Так как у меня уже создан GitHub с прошлого семестра, теперь нужно лишь подкорректировать некоторые моменты.

Верификация коммитов с помощью PGP. Создание ключа (рис. @fig:001).

![Создание ключа](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 17-46-50.png){#fig:001 width=70%}

Экспорт ключа (рис. @fig:002)

![Экспорт ключа](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-00-04.png){#fig:002 width=70%}

Экспортируем ключ в формате ASCII по его отпечатку (рис. @fig:003).

![PGP ключ](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-03-15.png){#fig:003 width=70%}

Добавление PGP ключа в GitHub (рис. @fig:004).

![добавление ключа](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-07-27.png){#fig:004 width=70%}

Настройка автоматических подписей коммитов git (рис. @fig:005).

![настройка](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-11-45.png){#fig:005 width=70%}

Настройка gh (рис. @fig:006),(рис. @fig:007), (рис. @fig:008).

![gh](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-14-06.png){#fig:006 width=70%}

![Авторизация ](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-26-04.png){#fig:007 width=70%}

![Авторизация](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-26-42.png){#fig:008 width=70%}

Создание репозитория курса на основе шаблона (рис. @fig:009).

![Репозиторий](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-37-47.png){#fig:009 width=70%}

Настройка каталога курса (рис. @fig:010), (рис. @fig:011).

![создание](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-43-09.png){#fig:010 width=70%}

![Завершение](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-45-19.png){#fig:011 width=70%}

![Проверка](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab02/report/image/Снимок экрана от 2023-02-17 18-49-25.png){#fig:012 width=70%}


# Контрольные вопросы
1. это программные инструменты, помогающие командам разработчиков управлять изменениями в исходном коде с течением времени.

2. 

# Выводы

Я изучила идеологию и применение средств контроля версий и освоила умения по работе с git.


