---
## Front matter
title: "Лабораторная работа №6"
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

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними.

# Теоретическое введение

*Функциональные клавиши mc*
- **F1** Вызов контекстно-зависимой подсказки
- **F2** Вызов пользовательского меню с возможностью создания и/или дополнения дополнительных функций
- **F3** Просмотр содержимого файла, на который указывает подсветка в активной панели (без возможности редактирования)
- **F4** Вызов встроенного в mc редактора для изменения содержания файла, на который указывает подсветка в активной панели
- **F5** Копирование одного или нескольких файлов, отмеченных в первой (активной) панели, в каталог, отображаемый на второй панели
- **F6** Перенос одного или нескольких файлов, отмеченных в первой (активной) панели, в каталог, отображаемый на второй панели
- **F7** Создание подкаталога в каталоге, отображаемом в активной панели
- **F8** Удаление одного или нескольких файлов (каталогов), отмеченных в первой (активной) панели файлов
- **F9** Вызов меню mc
- **F10** Выход из mc

# Выполнение лабораторной работы

**Задание по mc**

1. (рис. @fig:001).

![man mc](image/Arkh1.png){#fig:001 width=70%}

2. (рис. @fig:002).

![Структура и меню mc](image/Arkh2.png){#fig:002 width=70%}

3. (рис. @fig:003).

![Несколько операций в mc, используя управляющие клавиши](image/Arkh2.png){#fig:003 width=70%}

4. (рис. @fig:004).

![Основные команды меню правой панели](image/Arkh3.png){#fig:004 width=70%}

5. (рис. @fig:005).

![Возможности подменю Файл](image/Arkh5.png){#fig:005 width=70%}

6. (рис. @fig:006).

![Cредства подменю Команда](image/Arkh7.png){#fig:006 width=70%}

7. (рис. @fig:007).

![Подменю Настройки](image/Arkh8.png){#fig:007 width=70%}

**Задание по встроенному редактору mc**

1-3. (рис. @fig:008).

![Скопированный текст в файле](image/Arkh9.png){#fig:008 width=70%}

4. (рис. @fig:009)(рис. @fig:010)(рис. @fig:011).

![Скопированный текст в файле](image/Arkh10.png){#fig:009 width=70%}.

![Скопированный текст в файле](image/Arkh11.png){#fig:010 width=70%}.

![Скопированный текст в файле](image/Arkh12.png){#fig:011 width=70%}.

# Выводы

Освоены основные возможности командной оболочки Midnight Commander. Приобретены навыки практической работы по просмотру каталогов и файлов; манипуляций с ними.
