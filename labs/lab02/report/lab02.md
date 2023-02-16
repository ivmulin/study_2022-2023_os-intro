---
## Front matter
title: "Отчёт по лабораторной работе №2"
subtitle: "Система контроля версий git"
author: "Мулин Иван Владимирович"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
## bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: false # List of tables
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

## Цель работы
Цель данной лабораторной работы состоит в изучении применения средств контроля версий и приобретении практических умений по работе с системой git. В ходе выполнения работы будет создан репозиторий, который можно найти по адресу [https://github.com/ivmulin/study_2022-2023_os-intro](https://github.com/ivmulin/study_2022-2023_os-intro).

# Выполнение лабораторной работы

## Базовая настройка git

Прежде чем создать репозиторий, необходимо настроить git:

![Basic git setup](image/Рис.%201.png "Basic git setup")


## Создание ключей SSH и GPG
SSH-ключ есть пара ключей, которая необходима при подключения к серверу по протоколу SSH.
Создаём ключ командой `ssh-keygen -t rsa -b 4096`. Теперь необходимо установить соединение клиента с сервером [github](https://github.com/). Для этого копируем только что сгенерированный ключ, вставляем в окне создания нового SSH-ключа и нажимаем `Add SSH key`.

Затем создадим ключ GPG:

![Настройка ключей SSH и GPG](image/Рис.%202.png "Настройка ключей SSH и GPG")

## Настройка автоматических подписей git

На данном этапе необходимо настроить автоматические подписи git:

![Настройка автоматических подписей git](image/Рис.%203.png "Настройка автоматических подписей git")

## Дальнейшая настройка репозитория

Завершаем регистрацию:

![Завершение регистрации](image/Рис.%204.png "Завершение регистрации")

После этого необходимо создать структуру курса и добавить ответ на готовые лабораторные работы в созданный репозиторий.


## Ответы на контрольные вопросы

1. Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются?

_Ответ_: система, позволяющая работать нескольким людям над одним проектом.

2. Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия.

_Ответ_: хранилище (репозиторий) - директория, хранящая конкретный проект; коммит - текущее состояние рабочей копии; история - последовательность коммитов в порядке, в котором они добавлялись в репозиторий; рабочая копия - текущее состояние репозитория, которое находится в состоянии изменения.


3. Что представляют собой и чем отличаются централизованные и децентрализованные VCS? Приведите примеры VCS каждого вида.

_Ответ_: в централизованных VCS (Mercurial) все пользователи подключены к единому серверу; в децентрализованных VCS пользователи подключены к нескольким владельцам.


4. Опишите действия с VCS при единоличной работе с хранилищем.

_Ответ_: при единоличной работе с хранилищем все изменения, созданные пользователем, не влияют на общий репозиторий.

5. Опишите порядок работы с общим хранилищем VCS.

_Ответ_: из общего хранилища можно получать изменения проекта.


6. Каковы основные задачи, решаемые инструментальным средством git?

_Ответ_: git позволяет несольким людям работать над одним проектом.


7. Назовите и дайте краткую характеристику командам git.

_Ответ_: `add` - добавить файлы в коммит, `push` - отправить коммит на удалённый репозиторий; `pull` - импортировать проект с удалённого репозитория.


8. Приведите примеры использования при работе с локальным и удалённым репозиториями.

_Ответ_:


9. Что такое и зачем могут быть нужны ветви (branches)?

_Ответ_: создав новую ветвь, можно, не вредя проекту, работать над конкретной частью проекта.


10. Как и зачем можно игнорировать некоторые файлы при commit?

_Ответ_: some files may well be user specific.




# Заключение
В результате выполнения лабораторной и самостоятельной работ были получены прикладные навыки работы с системой контроля версий git, а значит, цель работы была достигнута.