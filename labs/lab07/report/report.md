---
## Front matter
title: "Внешний курс. Раздел 2"
subtitle: "Основы информационной безопасности"
author: "Малюга Валерия Васильевна"
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

Пройти второй блок курса "Основы кибербезопасности"

# Выполнение блока 2: Защита ПК/Телефона

## Шифрование диска

Шифрование диска — технология защиты информации, переводящая данные на диске в нечитаемый код, который нелегальный пользователь не сможет легко расшифровать. Соответственно, можно (рис. [-@fig:001]).

![Вопрос 3.1.1](image/23.png){#fig:001 width=70%}

Шифрование диска основано на симметричном шифровании (рис. [-@fig:002]).

![Вопрос 3.1.2](image/24.png){#fig:002 width=70%}

Отмечены программы, с помощью которых можно зашифровать жетский диск (рис. [-@fig:003]).

![Вопрос 3.1.3](image/25.png){#fig:003 width=70%}

## Пароли

Стойкий пароль - тот, который тяжлее подобрать, он должен быть со спец. символами и длинный (рис. [-@fig:004]).

![Вопрос 3.2.1](image/26.png){#fig:004 width=70%}

Все варианты, кроме менеджера паролей, совершенно не надежные (рис. [-@fig:005]).

![Вопрос 3.2.2](image/27.png){#fig:005 width=70%}

Капча нужна для проверки на то, что за экраном "не робот"(рис. [-@fig:006]).

![Вопрос 3.2.3](image/28.png){#fig:006 width=70%}

Опасно хранить пароли в открытом виде, поэтому хранят их хэши (рис. [-@fig:007]).

![Вопрос 3.2.4](image/29.png){#fig:007 width=70%}

Соль не поможет (рис. [-@fig:008]).

![Вопрос 3.2.5](image/30.png){#fig:008 width=70%}

Все приведенные меры защищают от утечек данных (рис. [-@fig:009]).

![НВопрос 3.2.6](image/31.png){#fig:009 width=70%}

## Фишинг

Фишинговые ссылки очень похожи на ссылки известных сервисов, но с некоторыми отличиями (рис. [-@fig:010]).

![Вопрос 3.3.1](image/32.png){#fig:010 width=70%}

Да, может, например, если пользователя со знакомым адресом взломали (рис. [-@fig:011]).

![Вопрос 3.3.2](image/33.png){#fig:011 width=70%}

## Вирусы. Примеры

Ответ дан в соответствии с определением (рис. [-@fig:012]).

![Вопрос 3.4.1](image/34.png){#fig:012 width=70%}

Троян маскируется под обычную программу (рис. [-@fig:013]).

![Вопрос 3.4.2](image/35.png){#fig:013 width=70%}

## Безопасность мессенджеров

При установке первого сообщения отправителем формируется ключ шифрования (рис. [-@fig:014]).

![Вопрос 3.5.1](image/36.png){#fig:014 width=70%}

Суть сквозного шифрования состоит в том, что сообзения передаются по узлам связи в зашифрованном виде (рис. [-@fig:015]).

![Вопрос 3.5.2](image/37.png){#fig:015 width=70%}

# Выводы

Был пройден второй блок курса "Основы кибербезопасности", изучены правила хранения паролей и основная информация о вирусах
