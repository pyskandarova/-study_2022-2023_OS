---
## Front matter
lang: ru-RU
title: Лабораторная работа №10
subtitle: Архитектура компьютеров
author:
  - Скандарова П. Ю.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 19 апреля 2023

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Скандарова Полина Юрьевна
  * Российский университет дружбы народов
  * [1132221815@pfur.ru](mailto:1132221815@pfur.ru)
  * <https://pyskandarova.github.io/ru/>

:::
::: {.column width="30%"}

![](./image/kulyabov.jpg)

:::
::::::::::::::

# Вводная часть

## Цели и задачи

Изучить основы программирования в оболочке ОС UNIX. Научится писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

## Выполнение лабораторной работы

Используя команды getopts grep, пишу командный файл, который анализирует командную строку с ключами:
– -iinputfile — прочитать данные из указанного файла;
– -ooutputfile — вывести данные в указанный файл;
– -pшаблон — указать шаблон для поиска;
– -C — различать большие и малые буквы;
– -n — выдавать номера строк.
а затем ищет в указанном файле нужные строки, определяемые ключом -p.

## Выполнение лабораторной работы

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Текст программы](./image/Arkh6.png)

:::
::: {.column width="50%"}

![Результат](./image/Arkh5.png)

:::
::::::::::::::

## Выполнение лабораторной работы

Пишу на языке Си программу, которая вводит число и определяет, является ли оно больше нуля, меньше нуля или равно нулю. Затем программа завершается с помощью функции exit(n), передавая информацию в о коде завершения в оболочку. Командный файл должен вызывать эту программу и, проанализировав с помощью команды $?, выдать сообщение о том, какое число было введено.

## Выполнение лабораторной работы

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Текст программы](./image/Arkh4.png)

:::
::: {.column width="50%"}

![Результат](./image/Arkh5.png)

:::
::::::::::::::

## Выполнение лабораторной работы

Пишу командный файл, создающий указанное число файлов, пронумерованных последовательно от 1 до N (например 1.tmp, 2.tmp, 3.tmp,4.tmp и т.д.). Число файлов, которые необходимо создать, передаётся в аргументы командной строки. Этот же командный файл должен уметь удалять все созданные им файлы (если они существуют).

## Выполнение лабораторной работы

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Текст программы](./image/Arkh6.png)

:::
::: {.column width="50%"}

![Результат](./image/Arkh5.png)

:::
::::::::::::::

## Выполнение лабораторной работы

Пишу командный файл, который с помощью команды tar запаковывает в архив 0все файлы в указанной директории. Модифицировать его так, чтобы запаковывались только те файлы, которые были изменены менее недели тому назад (использовать команду find).

## Выполнение лабораторной работы

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Текст программы](./image/Arkh4.png)

:::
::: {.column width="50%"}

![Результат](./image/Arkh5.png)

:::
::::::::::::::

## Результаты

Изучены основы программирования в оболочке ОС UNIX. Я научилась писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.


# Неспасибо за невнимание
