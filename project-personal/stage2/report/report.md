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

Добавить на сайт информацию 
Список добавляемых данных.
* Разместить фотографию владельца сайта.
* Разместить краткое описание владельца сайта (Biography).
* Добавить информацию об интересах (Interests).
** Добавить информацию от образовании (Education).
** Сделать пост по прошедшей неделе.
** Добавить пост на тему по выбору:
** Управление версиями. Git.
** Непрерывная интеграция и непрерывное развертывание (CI/CD).

# Выполнение лабораторной работы

## Добавляем биографию + фото

1. Добавил фото, перетащив его в нужную папку (рис. [-@fig:001]), добавил биографию (рис. [-@fig:002]), добавил свои навыки (рис. [-@fig:003]), добавил курсы (рис. [-@fig:004]).

![мое фото](image/1.png){#fig:001 width=70%}

![моя биография](image/2.png){#fig:002 width=70%}

![мои навыки](image/3.png){#fig:003 width=70%}

![мои курсы](image/4.png){#fig:004 width=70%}

## делаем посты

2. делаем пост про прощедшую неделю (рис. [-@fig:005]), делаем пост про Git (рис. [-@fig:006]).


![пост про прощедшую неделю](image/5.png){#fig:005 width=70%}

![пост про git](image/6.png){#fig:006 width=70%}


## Загрузка + проверка

3. Запуск hugo (рис. [-@fig:007]), загрузка на гитхаб + проверка (рис. [-@fig:008]) (рис. [-@fig:009]) (рис. [-@fig:0010]).

![hugo](image/7.png){#fig:007 width=70%}

![мои навыки + био](image/8.png){#fig:008 width=70%}

![мои курсы](image/9.png){#fig:009 width=70%}

![мои посты](image/10.png){#fig:010 width=70%}

# Выводы

Этап 2 пройден (добавленая биография и фото)

# Список литературы{.unnumbered}

::: {#refs}
:::
