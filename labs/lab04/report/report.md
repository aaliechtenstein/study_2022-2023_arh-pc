---
## Front matter
title: "ОТЧЕТ О ВЫПОЛНЕНИИ ЛАБОРАТОРНОЙ РАБОТЫ №4"
subtitle: "_дисциплина: Архитектура компьютера_"
author: "Лихтенштейн Алина Алексеевна"

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

# Цель работы

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

Перейдем в каталог курса, сформированный при выполнении лабораторной работы №3, обновим локальный репозиторий, скачав изменения из удаленного репозитория (рис. [-@fig:fig1])

![Обновление локального репозитория](image/1.png){ #fig:fig1 width=70% }

Перейдем в каталог с шаблоном отчета о выполнении лабораторной работы №4 и проведем компиляцию шаблона с использованием Makefile. Для этого введем команду make
При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx. Откроем и проверим корректность полученных файлов (рис. [-@fig:fig2])

![Компиляция шаблона](image/2.png){ #fig:fig2 width=70% }

При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx. Откроем и проверим корректность полученных файлов (рис. [-@fig:fig3])

![Проверка наличия скомпилированных файлов](image/3.png){ #fig:fig3 width=70% }

Удалим полученные файлы с использованием Makefile. Для этого введем команду make clean (рис. [-@fig:fig4])

![Удаление скомпилированных файлов](image/4.png){ #fig:fig4 width=70% }

Проверим, что после этой команды файлы report.pdf и report.docx были удалены. (рис. [-@fig:fig5])

![Проверка результата операции удаления скомпилированных файлов](image/5.png){ #fig:fig5 width=70% }

Откроем файл report.md c помощью текстового редактора gedit (рис. [-@fig:fig6], [-@fig:fig7])

![Команда в терминале для запуска файла report.md в текстовом редакторе gedit](image/6.png){ #fig:fig6 width=70% }

![Файл report.md в текстовом редакторе gedit](image/7.png){ #fig:fig7 width=70% }

Для корректного отображения скриншотов разместим их в каталоге image (рис. [-@fig:fig8])

![Каталог .../arch-pc/labs/lab04/report/image](image/8.png){ #fig:fig8 width=70% }

Загрузим файлы на Github (рис. [-@fig:fig9])

![Загрузка файлов на Github](image/9.png){ #fig:fig9 width=70% }

# Выполнение задания для самостоятельной работы

Ссылка на отчет о выполнении лабораторной работы №3 на GitHub: 
https://github.com/aaliechtenstein/study_2022-2023_arh-pc/tree/master/labs/lab03

Перейдем в каталог отчета о выполнении лабораторной работы №3 и выведем содержимое (рис. [-@fig:fig10])

![Переход в каталог .../arch-pc/labs/lab03/report и вывод содержимого](image/10.png){ #fig:fig10 width=70% }

Добавим в каталог .../arch-pc/labs/lab03/report/image все скриншоты, использовавшиеся в данном отчете (рис. [-@fig:fig11])

![Каталог .../arch-pc/labs/lab03/report/image с добавленными скриншотами](image/11.png){ #fig:fig11 width=70% }

Изменим содержимое report.md, где опишем отчет о выполнении лабораторной работы №3 (рис. [-@fig:fig12])

![Правка содержимого .../arch-pc/labs/lab03/report/report.md](image/12.png){ #fig:fig12 width=70% }

Проведем компиляцию шаблона с использованием Makefile (рис. [-@fig:fig13])

![Компиляция шаблона лабораторной работы №3](image/13.png){ #fig:fig13 width=70% }

Выведем содержимое каталога .../arch-pc/labs/lab03/report (рис. [-@fig:fig14])

![Вывод содержимого каталога](image/14.png){ #fig:fig14 width=70% }

# Выводы

В процессе выполнения лабораторной работы были получены практические навыки оформления отчетов с помощью легковесного языка разметки Markdown.
