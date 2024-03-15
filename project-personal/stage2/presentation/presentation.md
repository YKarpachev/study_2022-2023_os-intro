---
## Front matter
lang: ru-RU
title: Отчёт по 2 этапу индивидуального проекта
subtitle: Операционные системы
author:
  - Карпачев Ярослав
institute:
  - Российский университет дружбы народов, Москва, Россия
  - НБИбд-01-23
date: 14 марта 2024

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

## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
---

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Карпачев Ярослав Олегович
  * Студент 
  * НКАбд-01-23
  * Российский университет дружбы народов
  * [1132232862@pfur.ru](mailto:113222862@rudn.ru)

:::
::: {.column width="30%"}

![](image/avatar.jpeg)

:::
::::::::::::::
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

##
Добавил фото перетащив его в нужную папку
![мое фото](image/1.png)

##
добавил биографию 
![моя биография](image/2.png){#fig:002 width=70%}

##
добавил свои навыки
![мои навыки](image/3.png){#fig:003 width=70%}

##
добавил курсы
![мои курсы](image/4.png){#fig:004 width=70%}

## делаем посты

##
делаем пост про прощедшую неделю
![пост про прощедшую неделю](image/5.png)

##
делаем пост про Git
![пост про git](image/6.png)


## Загрузка + проверка

##
Запуск hugo 
![hugo](image/7.png)

##
загрузка на гитхаб + проверка.

![мои навыки + био](image/8.png)

![мои курсы](image/9.png)

![мои посты](image/10.png)

# Выводы

Этап 2 пройден (добавленая биография и фото)

# Список литературы{.unnumbered}

::: {#refs}
:::
