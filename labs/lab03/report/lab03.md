---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Markdown"
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

## Теоретическое введение

Markdown - система разметки текста. Позволяет быстро и удобно создавать текстовые отчёты, рефераты, презентации...

Для написания обычного текста достаточно его написать. Заголовки первого, второго, ... , шестого уровней выделяются в начале строке одним, двумя, ... , шестью симовлами `#`:
``` Markdown
# Заголовок первого уровня
## Подзаголовок
```

Для создания нумерованного списка нужно написать число с точкой (достаточно перед каждым пунктом писть `1.`):
``` Markdown
1. так
1. создаётся
1. длинный текст
1. Маяковский делал
1. так же
```

Для создания ненумерованного списка в начале строки нужно добавить один из маркеров, а именно: `*`, `-`, `+`.

## Цель работы
В ходе выполнения данной лабораторной работы необходимо изучить и применить на практике систему разметки текста Markdown. Репозиторий автора можно найти по адресу [https://github.com/ivmulin/study_2022-2023_os-intro](https://github.com/ivmulin/study_2022-2023_os-intro).

# Выполнение лабораторной работы

Выполнение данной лабораторной работы заключается в написании уже созданного [отчёта к лабораторной работе номер 2](https://github.com/ivmulin/study_2022-2023_os-intro/blob/master/labs/lab02/report/lab02.md).

# Заключение
В результате выполнения лабораторной работы была изучена технология разметки текста Markdown. Цель работы была достигнута.