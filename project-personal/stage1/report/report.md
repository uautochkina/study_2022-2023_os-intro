---
## Front matter
title: "Отчет по индивидуальному проекту. Этап №1"
subtitle: "Дисциплина: Операционные системы"
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
-—
# Цель работы

Размещение на GitHub pages заготовки для персонального сайта.

# Задачи

- Установить необходимое программное обеспечение.

- Скачать шаблон темы сайта.

- Разместить его на хостинге git.

- Установить параметр для URLs сайта.

- Разместить заготовку сайта на Github pages.

# Выполнение лабораторной работы

1. Скачала архив с репозитория. (рис. [-@fig:001]).

![Скачивание](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 17-32-30.png){#fig:001 width=70%}

2. Перенести hugo (рис. [-@fig:002]), (рис. [-@fig:003]).

![Копирование](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 17-36-04.png){#fig:002 width=70%}

![В папку bin](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 17-37-17.png){#fig:003 width=70%}

3. Создание репозитория blog (рис. [-@fig:004]).

![blog](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 17-41-36.png){#fig:004 width=70%}

4. Удаляем public (рис. [-@fig:005]).

![public](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 19-09-03.png){#fig:005 width=70%}

5. По ссылке открыла сайт (рис. [-@fig:006]).

![Сайт](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 19-31-30.png){#fig:006 width=70%}

6. Клонируем репозиторий (рис. [-@fig:007]).

![Клонирование](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 19-51-18.png){#fig:007 width=70%}

7. Создаем ветку и файл Readme (рис. [-@fig:008]).

![README](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 19-57-45.png){#fig:008 width=70%}

8. Добавляем public (рис. [-@fig:009]).

![public](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 20-07-09.png){#fig:009 width=70%}

9. Связываем. (рис. [-@fig:010]).

![github.io](/home/uautochkina/work/study/2022-2023/Операционные системы/os-intro/project-personal/stage1/report/image/Снимок экрана от 2023-02-22 20-09-35.png){#fig:010 width=70%}

# Вывод

В результате лабораторной работы мы разместилиа на GitHub pages заготовки для персонального сайта.

# Список литературы{.unnumbered}

1. [https://www.youtube.com/watch?v=OpsSv0RE3C4](https://www.youtube.com/watch?v=OpsSv0RE3C4)


::: {#refs}
:::

