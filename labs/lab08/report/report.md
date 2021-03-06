---
## Front matter
title: "Отчёт по лабораторной работе №8"
subtitle: "Текстовой редактор vi"
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание 1

1. Создайте каталог с именем ~/work/os/lab06.
2. Перейдите во вновь созданный каталог.
3. Вызовите vi и создайте файл hello.sh
1 vi hello.sh
4. Нажмите клавишу i и вводите следующий текст.
1 #!/bin/bash
2 HELL=Hello
3 function hello {
4 LOCAL HELLO=World
5 echo $HELLO
6 }
7 echo $HELLO
8 hello
5. Нажмите клавишу Esc для перехода в командный режим после завершения ввода
текста.
6. Нажмите : для перехода в режим последней строки и внизу вашего экрана появится
приглашение в виде двоеточия.
7. Нажмите w (записать) и q (выйти), а затем нажмите клавишу Enter для сохранения
вашего текста и завершения работы.
8. Сделайте файл исполняемым
1 chmod +x hello.sh

# Задание 2

1. Вызовите vi на редактирование файла
1 vi ~/work/os/lab06/hello.sh
2. Установите курсор в конец слова HELL второй строки.
3. Перейдите в режим вставки и замените на HELLO. Нажмите Esc для возврата в командный режим.
4. Установите курсор на четвертую строку и сотрите слово LOCAL.
5. Перейдите в режим вставки и наберите следующий текст: local, нажмите Esc для
возврата в командный режим.
6. Установите курсор на последней строке файла. Вставьте после неё строку, содержащую
следующий текст: echo $HELLO.
7. Нажмите Esc для перехода в командный режим.
8. Удалите последнюю строку.
9. Введите команду отмены изменений u для отмены последней команды.
10. Введите символ : для перехода в режим последней строки. Запишите произведённые
изменения и выйдите из vi.

# Выполнение лабораторной работы. Задание 1

Создаю каталог с именем  ~/work/os/lab06, перехожу туда и вызываю vi, создаю файл hello.sh

![hello.sh](image/1.png)

##

Нажимаю клавишу i и ввожу текст из задания

![текст](image/2.png)

##

 Нажимаю клавишу Esc, чтобы перейти в командный режим, а затем нажимаю : для перехода в режим последней строки

![Esc & :](image/3.png)

##

 Нажимаю w и q для записи и выхода, затем нажимаю enter для сохранения файла

![сохранение файла](image/4.png)

##

 Делаю файл исполняемым

![исполняемый файл](image/5.png)

# Выполнение лабораторной работы. Задание 2

 Вызываю vi на редактирование файла
 
![редактирование](image/6.png)

##

 Устанавливаю курсор на конец строки слова HELL второй строки, а затем перехожу в режим вставки и заменяю на HELLO.

![замена](image/7.png)

##

 Устанавливаю курсор на четвертую строку и стираю слово LOCAL, перехожу в режим вставки и ввожу local.

![замена](image/8.png)

##

 Устанавливаю курсор на последней строке файла и вставляю после неё строку с текстом echo $HELLO

![повторение строки](image/9.png)

##

 Удаляю последнюю строку командой 9d (номер строки и удаление)


![удаление строки](image/10.png)

##

 Ввожу команду отмены изменений u для отмены последней команды

![отмена команды](image/11.png)

##

 Ввожу символ : для перехода в режим последней строки, а затем записываю и выхожу из vi командой wq

![запись и выход](image/12.png)

# Контрольные вопросы


1.  Редактор vi имеет три режима работы:

-   командный режим − предназначен для ввода команд редактирования и навигации по редактируемому файлу;
-   режим вставки - предназначен для ввода содержания редактируемого файла;
-   режим последней (или командной) строки − используется для записи изменений в файл и выхода из редактора.

2.  Чтобы выйти из редактора, не сохраняя произведённые изменения, нужно в режиме командной строки нажать клавиши «:» «q» «!»
3.   Команды позиционирования:

-   «0» (ноль) − переход в начало строки;
-   «$» − переход в конец строки;
-   «G» − переход в конец файла;
-   n «G» − переход на строку с номером n.

4.  При использовании прописных W и B под разделителями понимаются только пробел, табуляция и возврат каретки. При использовании строчных w и b под разделителями понимаются также любые знаки пунктуации.
5.  Чтобы из любого места редактируемого файла перейти в начало (конец) файла, нужно в режиме командной строки нажать клавиши «1» «G» («G»).
6.  Команды редактирования:
    Вставка текста

-   «а» − вставить текст после курсора;
-   «А» − вставить текст в конец строки;
-   «i» − вставить текст перед курсором;
-   n «i» − вставить текст n раз;
-   «I» − вставить текст в начало строки.
    Вставка строки
-   «о» − вставить строку под курсором;
-   «О» − вставить строку над курсором.
    Удаление текста
-   «x» − удалить один символ в буфер;
-   «d» «w» − удалить одно слово в буфер;
-   «d» «$» − удалить в буфер текст от курсора до конца строки;
-   «d» «0» − удалить в буфер текст от начала строки до позиции курсора;
-   «d» «d» − удалить в буфер одну строку;
-   n «d» «d» − удалить в буфер n строк.
    Отмена и повтор произведённых изменений
-   «u» − отменить последнее изменение;
-   «.» − повторить последнее изменение.Копирование текста в буфер
-   «Y» − скопировать строку в буфер;
-   n «Y» − скопировать n строк в буфер;
-   «y» «w» − скопировать слово в буфер.
    Вставка текста из буфера
-   «p» − вставить текст из буфера после курсора;
-   «P» − вставить текст из буфера перед курсором.
    Замена текста
-   «c» «w» − заменить слово;
-   n «c» «w» − заменить n слов;
-   «c» «$» − заменить текст от курсора до конца строки;
-   «r» − заменить слово;
-   «R» − заменить текст.
    Поиск текста
-   «/» текст − произвести поиск вперёд по тексту указанной строки символов текст;
-   «?» текст − произвести поиск назад по тексту указанной строки символов текст.
-   Копирование и перемещение текста
-   «:» n,m «d» – удалить строки с n по m;
-   «:» i,j «m» k – переместить строки с i по j, начиная со строки k;
-   «:» i,j «t» k – копировать строки с i по j в строку k;
-   «:» i,j «w» имя-файла – записать строки с i по j в файл с именем имя-файла.-
7.  Чтобы заполнить строку символами $, необходимо для начала перейти на эту строку, нажав клавиши n «G», где n – номер строки, далее нажать «0» для перехода в начало строки. Теперь необходимо нажать «c» «$», чтобы заменить текст от курсора до конца строки, и ввести символы $.
8.  Чтобы отменить по одному предыдущему действию последовательно,необходимо нажать «u». Чтобы отменить все изменения, произведённые со времени последней записи, нужно нажать «:» «e» «!».
9.  Команды редактирования в режиме командной строки
    Копирование и перемещение текста

-   «:» n,m «d» − удалить строки с n по m;
-   «:» i,j «m» k − переместить строки с i по j, начиная со строки k;
-   «:» i,j «t» k − копировать строки с i по j в строку k;
-   «:» i,j «w» имя-файла − записать строки с i по j в файл с именем имя-файла.
    Запись в файл и выход из редактора
-   «:» «w» − записать изменённый текст в файл, не выходя из vi;
-   «:» «w» имя-файла − записать изменённый текст в новый файл с именем имя-файла;
-   «:» «w» «!» имя-файла − записать изменённый текст в файл с именем имя-файла;
-   «:» «w» «q» − записать изменения в файл и выйти из vi;
-   «:» «q» − выйти из редактора vi;
-   «:» «q» «!» − выйти из редактора без записи;
-   «:» «e» «!» − вернуться в командный режим, отменив все изменения, произведённые со времени последней записи.
    Опции
-   Опции редактора vi позволяют настроить рабочую среду. Для задания опций используется команда set (в режиме последней строки):
-   «:» set all − вывести полный список опций;
-   «:» set nu − вывести номера строк;
-   «:» set list − вывести невидимые символы;
-   «:» set ic − не учитывать при поиске, является ли символ прописным или строчным.
    Если вы хотите отказаться от использования опции, то в команде setперед именем опции надо поставить no.

10.   Чтобы определить, не перемещая курсора, позицию, в которой заканчивается строка, нужно в командном режиме находясь на нужной строке нажать «$» и посмотреть на число после запятой в правом нижнем углу экрана.
11.   Опции редактора vi позволяют настроить рабочую среду. Для задания опций используется команда set (в режиме командной строки). Если вы хотите отказаться от использования опции, то в команде set перед именем опции надо поставить no.
12.   Чтобы просмотреть опции редактора vi, необходимо нажать «:» set all. Нажав «:» help “название_опции”, можно узнать назначение конкретной опции.
    В режиме командной строки внизу редактора присутствует «:», в режиме ввода – «-- ВСТАВКА --», в командном режиме внизу ничего нет.
13.   Граф взаимосвязи режимов работы редактора vi.


# Выводы

В ходе выполнения лабораторной работы №8 я познакомилась с операционной системой Linux и получила практические навыки работы с редактором vi.

