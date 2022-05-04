---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Операционные системы"
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

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задание

1. Определите полное имя вашего домашнего каталога.Далее относительно этого ката-лога будут выполняться последующие упражнения.
2. Выполните следующие действия:
 2.1. Перейдите в каталог/tmp.
 2.2.Выведите на экран содержимое каталога/tmp.Для этого используйте команду ls с различными опциями.Поясните разницу в выводимой на экран информации.
 2.3. Определите,естьли в каталоге /var/spool подкаталог с именем cron?
 2.4.Перейдите в Ваш домашний каталог и выведите на экран его содержимое.Опре-делите,кто является владельцем файлов и подкаталогов.
3. Выполните следующие действия:
 - 3.1. В домашнем каталоге создайте новый каталог с именем newdir.
 - 3.2. В каталоге~/newdirсоздайте новый каталог с именем morefun.
 - 3.3.В домашнем каталоге создайте одной командой три новых каталога с именами letters,memos,misk.Затем удалите эти каталоги одной командой.
 - 3.4.Попробуйте удалить ранее созданный каталог~/newdir командой rm.Проверьте,был ли каталог удалён.
 - 3.5.Удалите каталог~/newdir/morefun из домашнего каталога.Проверьте,был ли каталог удалён.
4. С помощью команды man определите, какую опцию команды ls нужно использовать для просмотра содержимое нетолько указанного каталога,но и подкаталогов,входящих в него.
5. Спомощью команды man определите набор опций команды ls,позволяющийотсортировать по времени последнего изменения выводимый список содержимого каталогас развёрнутым описанием файлов.
6. Используйте команду man для просмотра описания следующих команд:cd,pwd,mkdir,rmdir,rm.Поясните основные опции этих команд.
7. Используя информацию,полученную при помощи команды history,выполните модификацию и исполнение нескольких команд из буфера команд.


# Выполнение лабораторной работы

Определение полного имени домашнего каталога
![каталог](image/1.png)

Переходим в каталог /tmp и и выводим его содержимое двумя способами
![каталог tmp](image/2.png)

Опредеяем есть ли в каталоге /var/spool подкаталог cron
![каталог /var/spool](image/3.png)

Перехожу  в домашний каталог и вывожу содержимое и определяю кто владелец каталогов (я)
![домашний каталог](image/4.png)

В домашнем каталоге создаю новый каталог newdir, а в нём новый каталог morefun. Далее создаю одной командой три новых каталога letters,memos,misk. Затем удаляю так же одной командой
![три каталога](image/5.png)

Пробую удалить каталог newdir и проверяю, удалён ли он
![удаление каталога](image/6.png)

Командой man определяю опции команды ls
![man](image/7.png)

Так же поступаю и с командами cd,pwd,mkdir,rmdir,rm
![else](image/8.png)

Выполеняю модификацию history
![history](image/9.png)
![history](image/10_0.png)
![history](image/10.png)

# Выводы

В ходе выполнения лабораторной работы №4 я приобрела практические навыки взаимодействия пользователя с системой посредством командной строки.

# Список литературы{.unnumbered}

::: {#refs}
:::
