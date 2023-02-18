---
## Front matter
title: "Отчёт по лабораторной работе №1"
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
Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.


# Выполнение лабораторной работы
Установили виртуальную машину еще в прошлом семестре. А также настроили каталог для нее.

Обнивила все пакеты (рис. @fig:001), (рис. @fig:002).

![обновление начало](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/Снимок экрана от 2023-02-16 11-44-39.png){#fig:001 width=70%}

![обновление конец](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/Снимок экрана от 2023-02-17 19-14-55.png){#fig:002 width=70%}

Установка программы для удобства работы в консоли, а также отключение SELinux (рис. @fig:003).

![tmux and SELinux](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/Снимок экрана от 2023-02-17 19-35-01.png){#fig:003 width=70%}

Установка драйыеров и DKMS(рис. @fig:004), @fig:005).

![Установка драйвером](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/Снимок экрана от 2023-02-17 19-41-41.png){#fig:004 width=70%}

![DKMS](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/Снимок экрана от 2023-02-17 23-28-50.png){#fig:005 width=70%}


# Выполнение домашней работы
Проанализировали последовательность загрузки и  нашли информацию по следующим вопросам: 
        Версия ядра Linux (Linux version).
        Частота процессора (Detected Mhz processor).
        Модель процессора (CPU0).
        Объём доступной оперативной памяти (Memory available).
        Тип обнаруженного гипервизора (Hypervisor detected).
        Тип файловой системы корневого раздела.
        Последовательность монтирования файловых систем.

(рис. @fig:006).

![домашнее задание](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/labs/lab01/report/image/Снимок экрана от 2023-02-17 23-55-37.png){#fig:006 width=70%}

# Контрольные вопросы

1. user name, UID,GID,password,full name,home directory,login shell

2. для получения справки по команде;help
для перемещения по файловой системе; cd
для просмотра содержимого каталога;ls
для определения объёма каталога;du
для создания / удаления каталогов / файлов;mkdir/rm -r
для задания определённых прав на файл / каталог;touch/rm
для просмотра истории команд.history

3. Файловая система — порядок, определяющий способ организации, хранения и именования данных на носителях информации в компьютерах, а также в другом электронном оборудовании: цифровых фотоаппаратах, мобильных телефонах и т.

4. Df

5. killall-killall()
# Выводы
Приобреда навыки необходимые для дальнейшей паботы



::: {#refs}
:::
