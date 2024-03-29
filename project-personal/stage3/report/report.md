---
## Front matter
title: "Персональный проект"
subtitle: "Стадия 2"
author: "Карпачев Ярослав"

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

Продолжить работы со своим сайтом. Редактировать его в соответствии с требованиями. Добавить данные о себе.

# Задание

Добавить к сайту достижения.
- Список достижений.
1. Добавить информацию о навыках (Skills).
2. Добавить информацию об опыте (Experience).
3. Добавить информацию о достижениях (Accomplishments).
- Сделать пост по прошедшей неделе.
- Добавить пост на тему по выбору:
1. Легковесные языки разметки.
2. Языки разметки. LaTeX.
3. Язык разметки Markdown.

# Выполнение лабораторной работы

## Добавляем skills, опыт работы, достижения (изменяя markdown файл.)

1. Добавил skills (рис. [-@fig:001]).

![мои навыки](image/1.png){#fig:001 width=70%}

2. Добавил опыт работы (рис. [-@fig:002]).

![мои навыки](image/2.png){#fig:002 width=70%}

3. Добавил достижения (рис. [-@fig:003]).

![мои навыки](image/3.png){#fig:003 width=70%}

## Добавляем посты

1. делаем пост про прощедшую неделю 2 (рис. [-@fig:004]), делаем пост про Git (рис. [-@fig:005]).

![пост про прощедшую неделю](image/4.png){#fig:004 width=70%}

![пост про git](image/5.png){#fig:005 width=70%}


## Загрузка + проверка

1. Запуск hugo (рис. [-@fig:006]), загрузка на гитхаб + проверка (рис. [-@fig:007]) (рис. [-@fig:009]) (рис. [-@fig:008]) (рис. [-@fig:009]).

![hugo](image/6.png){#fig:006 width=70%}

![github](image/7.png){#fig:007 width=70%}

![github](image/8.png){#fig:007 width=70%}

![github](image/9.png){#fig:007 width=70%}

# Выводы

Этап 3 пройден (добавлены способности, опыт, достижения)
