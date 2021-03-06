---
## Front matter
lang: ru-RU
title: Средства, применяемые при разработке программного обеспечения в ОС типа UNIX/Linux
author: |
	Федюшина Ярослава Андреевна
institute: |
	Российский Университет Дружбы Народов


## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Цель работы

Приобрести простейшие навыки разработки, анализа, тестирования и отладки приложений в ОС типа UNIX/Linux на примере создания на языке программирования С калькулятора с простейшими функциями.


# Выполнение лабораторной работы

В домашнем каталоге создаю подкаталог ~/work/os/lab_prog.

##

![lab_prog](image/1.png)

##

Создаю в нём файлы calculate.h, calculate.c и main.c

##

![создание файлов](image/2.png)

##

Реализация функций калькулятора в файле calculate.h

##

![calculate.h](image/3.png)

##

Интерфейсный файл calculate.h, описывающий формат вызова функции калькулятора

##

![calculate.h](image/4.png)

##

Основной файл main.c, реализующий интерфейс пользователя калькулятору

##

![main.c](image/4.1.png)

##

Далее выполняю компиляцию программы посредством gcc

##

![компиляция программы](image/5.png)

![.](image/6.png)

![сами файлы](image/7.png)

##

Создаю Makefile

##

![код makefile](image/8.png)

##

Далее исправляю код для Makefile

##

![исправление кода](image/9.png)

##

С помощью gdb выполняю отладку программы calcul и запускаю отладчик GDB, загрузив в него программу для отладки. Для запуска ввожу команду run

##

![запуск отладчика](image/10.png)

# Выводы

В ходе выполнения лабораторной работы №13 я приобрела простейшие навыки разработки, анализа, тестирования и отладки приложений в ОС типа UNIX/Linux на примере создания на языке программирования С калькулятора с простейшими функциями 
