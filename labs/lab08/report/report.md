---
## Front matter
title: "Лабораторная работа №8"
subtitle: "Архитектура компьютеров"
author: "Скандарова Полина"

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

# Теоретическое введение

**Команды позиционирования**
- 0 (ноль) — переход в начало строки;
- $ — переход в конец строки;
- G — переход в конец файла;
- n G — переход на строку с номером n.

**Команды перемещения по файлу**
- Ctrl-d — перейти на пол-экрана вперёд;
- Ctrl-u — перейти на пол-экрана назад;
- Ctrl-f — перейти на страницу вперёд;
- Ctrl-b — перейти на страницу назад.

**Команды перемещения по словам**
- W или w — перейти на слово вперёд;
- n W или n w — перейти на n слов вперёд;
- b или B — перейти на слово назад;
- n b или n B — перейти на n слов назад.

***Команды редактирования***
**Вставка текста** 
- а — вставить текст после курсора;
- А — вставить текст в конец строки;
- i — вставить текст перед курсором;
- n i — вставить текст n раз;
- I — вставить текст в начало строки.

**Вставка строки**
- о — вставить строку под курсором;
- О — вставить строку над курсором.

**Удаление текста**
- x — удалить один символ в буфер;
- d w — удалить одно слово в буфер;
- d $ — удалить в буфер текст от курсора до конца строки;
- d 0 — удалить в буфер текст от начала строки до позиции курсора;
- d d — удалить в буфер одну строку;
- n d d — удалить в буфер n строк.

# Выполнение лабораторной работы

***Задание 1. Создание нового файла с использованием vi***

Cоздаю каталог с именем ~/work/os/lab08, перехожу во вновь созданный каталог и вызываю vi и создаю файл hello.sh (рис. @fig:001).

![vi hello.sh](image/Arkh1.png){#fig:001 width=70%}

Жму клавишу i и ввожу следующий текст (рис. @fig:002).

![Следующий текст](image/Arkh2.png){#fig:002 width=70%}

Жму клавишу Esc для перехода в командный режим после завершения ввода текста, жму : для перехода в режим последней строки и внизу экрана появляется приглашение в виде двоеточия, жму w (записать) и q (выйти), а затем клавишу Enter для сохранения текста и завершения работы (рис. @fig:003).

![wq](image/Arkh3.png){#fig:003 width=70%}

Делаю файл исполняемым(рис. @fig:004).

![chmod +x hello.sh](image/Arkh4.png){#fig:004 width=70%}

***Задание 2. Редактирование существующего файла***

Вызываю vi на редактирование файла, устанавливаю курсор в конец слова HELL второй строки, перехожу в режим вставки и заменяю на HELLO. Жму Esc для возврата в командный режим. Устанавливаю курсор на четвертую строку и стираю слово LOCAL. Перехожу в режим вставки и набираю следующий текст: local, жму Esc для возврата в командный режим. Устанавливаю курсор на последней строке файла. Вставляю после неё строку, содержащую следующий текст: echo $HELLO. Жму Esc для перехода в командный режим. Удаляю последнюю строку. Ввожу команду отмены изменений u для отмены последней команды. Ввожу символ : для перехода в режим последней строки. Записываю произведённые изменения и выхожу из vi (рис. @fig:005) (рис. @fig:006).

![vi](image/Arkh5.png){#fig:005 width=70%}

![vi :u](image/Arkh6.png){#fig:006 width=70%}

# Выводы

Я познакомилась с операционной системой Linux. Получила практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.
