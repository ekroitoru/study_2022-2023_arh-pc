---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Простейший вариант"
author: "Дмитрий Сергеевич Кулябов"

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

Целью работы является освоение процедуры оформления отчетов с помощью
легковесного языка разметки Markdown.

# Задание

1. Откройте терминал
2. Перейдите в каталог курса сформированный при выполнении лаборатор-
ной работы No3:cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc/
Обновите локальный репозиторий, скачав изменения из удаленного репози-
тория с помощью команды
git pull
3. Перейдите в каталог с шаблоном отчета по лабораторной работе No 3
cd ~/work/study/2022-2023/"Архитектура
компьютера"/arch-pc/labs/lab04/report↪
4. Проведите компиляцию шаблона с использованием Makefile. Для этого
введите команду
make
При успешной компиляции должны сгенерироваться файлы report.pdf и
report.docx. Откройте и проверьте корректность полученных файлов.
5. Удалите полученный файлы с использованием Makefile. Для этого введите
команду
make clean
Проверьте, что после этой команды файлы report.pdf и report.docx были
удалены.
6. Откройте файл report.md c помощью любого текстового редактора, на-
пример gedit
gedit report.md
Внимательно изучите структуру этого файла.
7. Заполните отчет и скомпилируйте отчет с использованием Makefile. Про-
верьте корректность полученных файлов. (Обратите внимание, для кор-
ректного отображения скриншотов они должны быть размещены в ката-
логе image)
8. Загрузите файлы на Github.
cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc
git add .
git commit -am 'feat(main): add files lab-3'
git push
# Теоретическое введение
Markdown — язык текстовой разметки, созданный писателем и блогером Джоном Грубером. Он предназначен для создания красиво оформленных текстов в обычных файлах формата TXT. 
# Выполнение лабораторной работы

1-2 обновляем локальный репозиторий (рис. [-@fig:001])

![выполнение команды](image/placeimg_скрин1.jpg){ #fig:001 width=70% }

3 переход в каталог с шаблоном отчета по лабораторной работе No 4 (рис. [-@fig:002])

![выполнение команды](image/placeimg_скрин2.jpg){ #fig:002 width=70% }

4 проведение копиляции и сгенерирования файлов (рис. [-@fig:003])(рис. [-@fig:004])

![выполнение команды](image/placeimg_скрин3.jpg){ #fig:003 width=70% }  (image/placeimg_скрин4.jpg){ #fig:004 width=70% } 

проверка коректности полученный файлов (рис. [-@fig:005])
(image/placeimg_скрин5.jpg){ #fig:005 width=70% }

5 удаление полученный файлов (рис. [-@fig:006])

![выполнение команды](image/placeimg_скрин6.jpg){ #fig:006 width=70% }

проверка коректности выполнения команды (рис. [-@fig:007])

![выполнение команды](image/placeimg_скрин7.jpg){ #fig:007 width=70% }

открытие редактора  (рис. [-@fig:008])

![выполнение команды](image/placeimg_скрин8.jpg){ #fig:008 width=70% }


# Выводы

Мы освояли процедуры оформления отчетов с помощью
легковесного языка разметки Markdown.

::: {#refs}
:::
