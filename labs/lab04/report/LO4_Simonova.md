---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: ""
author: "Симонова Виктория Игоревна"

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

Получение навыков правильной работы с репозиториями git. Конкретно в данной лабораторной работе мы работаем с  gitflow  это определённая надстройка над моделью git.

# Задание

* Выполнить работу для тестового репозитория.
* Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.

# Теоретическое введение


* Gitflow Workflow опубликована и популяризована Винсентом Дриссеном.
* Gitflow Workflow предполагает выстраивание строгой модели ветвления с учётом выпуска проекта.
* Данная модель отлично подходит для организации рабочего процесса на основе релизов.
* Работа по модели Gitflow включает создание отдельной ветки для исправлений ошибок в рабочей среде.
* Последовательность действий при работе по модели Gitflow:
+ Из ветки master создаётся ветка develop.
+ Из ветки develop создаётся ветка release.
+ Из ветки develop создаются ветки feature.
+ Когда работа над веткой feature завершена, она сливается с веткой develop.
+ Когда работа над веткой релиза release завершена, она сливается в ветки develop и master.
+ Если в master обнаружена проблема, из master создаётся ветка hotfix.
+ Когда работа над веткой исправления hotfix завершена, она сливается в ветки develop и master.


# Выполнение лабораторной работы

## Установка git-flow

Установка из коллекции репозиториев Copr (рис. [-@fig:001]).

![Установка git-flow](image/1.png){#fig:001 width=70%}

## Установка Node.js

На Node.js базируется программное обеспечение для семантического версионирования и общепринятых коммитов.(рис. [-@fig:002]).

![Установка Node.js](image/3.png){#fig:002 width=70%}

Выполняю команды (рис. [-@fig:003]).

![Установка Node.js](image/4.png){#fig:003 width=70%}

## Настройка Node.js

Для работы с Node.js добавляю каталог с исполняемыми файлами, устанавливаемыми yarn, в переменную PATH.Запускаю установку (рис. [-@fig:004]).

![Настройка Node.js](image/5.png){#fig:004 width=70%}

Выполняю команду source ~/.bashrc (рис. [-@fig:005]).

![Настройка Node.js](image/6.png){#fig:005 width=70%}

## Общепринятые коммиты

Устанавливаю commitizen.Данная программа используется для помощи в форматировании коммитов.(скрипт git cz)(рис. [-@fig:006]).

![Установка программы](image/7.png){#fig:006 width=70%}

Устqанавливаю standard-changelog. Данная программа используется для помощи в создании логов.(рис. [-@fig:007]).

![Установка программы](image/8.png){#fig:007 width=70%}

Создаю новый git репозиторий (рис. [-@fig:008]).

![Создание репозитория](image/9.png){#fig:008 width=70%}

Клонирую репощиторий к себе на компьютер делаею первый коммит и выкладываю на github (рис. [-@fig:009]).

![Создание репозитория](image/10.png){#fig:009 width=70%}

Конфигурация для пакетов Node.js (рис. [-@fig:010]).

![Конфигурация общепринятых коммитов](image/11.png){#fig:010 width=70%}

Изменяю файл package.json (рис. [-@fig:011]).

![Изменяю файл](image/12.png){#fig:011 width=70%}

Добавляю новые файлы выполняю коммит и отправляю на github (рис. [-@fig:012]).

![Отправка на github](image/13.png){#fig:012 width=70%}

Инициализируем git-flow (рис. [-@fig:013]).

![Инициализация](image/14.png){#fig:013 width=70%}

Проверяю ветку и загружаю репощиторий в хранилище (рис. [-@fig:014]).

![Загрузка репозитория](image/15.png){#fig:014 width=70%}

Установливаю внешнюю ветку как вышестоящую для этой ветки. Создадаю релиз с версией 1.0.0. Создадаю журнал изменений. Добавляю журнал изменений в индекс (рис. [-@fig:015]).

![Установка внешней ветки](image/16.png){#fig:015 width=70%}

Заливаю релизную ветку в основную (рис. [-@fig:016]).

![Сливаю ветки](image/17.png){#fig:016 width=70%}

Обозначаю цель изменений (рис. [-@fig:017]).

![Комментарии](image/18.png){#fig:017 width=70%}

Вижу сообщение об успешном завершении процесса (рис. [-@fig:018]).

![Завершение](image/19.png){#fig:018 width=70%}

Отправляю данные на github и создаю релиз (рис. [-@fig:019]).

![Отправка файлов](image/20.png){#fig:019 width=70%}

Проверяю созданный релиз вводя полученную ссылку в адресную строку (рис. [-@fig:020]).

![Готовый релиз](image/21.png){#fig:020 width=70%}

Создадю ветку для новой функциональности и сразу же объелиняю её с веткой разработки (рис. [-@fig:021]).

![Новая ветка](image/22.png){#fig:021 width=70%}

Создаю релиз с версией 1.2.3 (рис. [-@fig:022]).

![Новый релиз](image/23.png){#fig:022 width=70%}

Изменяю номер версии в файле package.json. (рис. [-@fig:023]).

![Новый номер релиза](image/24.png){#fig:023 width=70%}

Создадаю журнал изменений. Добавляю журнал изменений в индекс.Отправляю данные (рис. [-@fig:024]).

![Новый номер релиза](image/25.png){#fig:024 width=70%}

Отправляю данные на github. Создаю релиз на github с комментарием из журнала изменений  (рис. [-@fig:025]).

![Новый номер релиза](image/26.png){#fig:025 width=70%}

Проверяю созданный релиз вводя полученную ссылку в адресную строку (рис. [-@fig:026]).

![Готовый релиз](image/27.png){#fig:026 width=70%}

# Выводы

Получила практические навыки работы с репозиториями git 

# Список литературы{.unnumbered}

1. Dash, P. Getting Started with Oracle VM VirtualBox / P. Dash. – Packt Publishing Ltd, 2013. – 86 сс.
2. Colvin, H. VirtualBox: An Ultimate Guide Book on Virtualization with VirtualBox. VirtualBox / H. Colvin. – CreateSpace Independent Publishing Platform, 2015. – 70 сс.
3. Vugt, S. van. Red Hat RHCSA/RHCE 7 cert guide : Red Hat Enterprise Linux 7 (EX200 and EX300) : Certification Guide. Red Hat RHCSA/RHCE 7 cert guide / S. van Vugt. – Pearson IT Certification, 2016. – 1008 сс.
4. Робачевский, А. Операционная система UNIX / А. Робачевский, С. Немнюгин, О. Стесик. – 2-е изд. – Санкт-Петербург : БХВ-Петербург, 2010. – 656 сс.
5. Немет, Э. Unix и Linux: руководство системного администратора. Unix и Linux / Э. Немет, Г. Снайдер, Т.Р. Хейн, Б. Уэйли. – 4-е изд. – Вильямс, 2014. – 1312 сс.
6. Колисниченко, Д.Н. Самоучитель системного администратора Linux : Системный администратор / Д.Н. Колисниченко. – Санкт-Петербург : БХВ-Петербург, 2011. – 544 сс.
7. Robbins, A. Bash Pocket Reference / A. Robbins. – O’Reilly Media, 2016. – 156 сс.

