---
## Front matter
title: "Отчёт по лабораторной работе №14"
subtitle: "Именованные каналы"
author: "Федюшина Ярослава Андреевна"

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

Приобретение практических навыков работы с именованными каналами

# Задание

1. Титульный лист с указанием номера лабораторной работы и ФИО студента.
2. Формулировка цели работы.
3. Описание результатов выполнения задания:
- скриншоты (снимки экрана), фиксирующие выполнение лабораторной работы;
- листинги (исходный код) программ (если они есть);
- результаты выполнения программ (текст или снимок экрана в зависимости от
задания).
4. Выводы, согласованные с целью работы.
5. Ответы на контрольные вопросы.

# Выполнение лабораторной работы

Создаю все нужные мне файлы

![создание файлов](image/1.png)

##

Далее я пишу коды для программ:

- common.h

##

![common.h](image/2.png)

##

- server.c

##

![server.c](image/3.png)

##

- client.c

##

![client.c](image/4.png)

##

- makefile

##

![makefile](image/5.png)

##

Использую команду make all, компилирую файлы

##

![компиляция](image/6.png)

![компиляция](image/7.png)

![все файлы в каталоге](image/8.png)

##

Проверяю на работу мой код и запускаю команды ./client и ./server

##

![проверка кода](image/10.png)


# Выводы

В ходе выполнения лабораторной работы №14 приобрела практические навыки работы с именованными каналами
