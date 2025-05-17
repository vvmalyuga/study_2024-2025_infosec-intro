---
## Front matter
title: "Внешний курс. Раздел 3"
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

Пройти третий блок курса "Основы кибербезопасности"

# Выполнение блока 3: Криптография на практике

## Введение в криптографию
 
Для ответа на вопрос используется определение ассмиетричного шифрования с двумя ключами (рис. [-@fig:001]).

![Вопрос 4.1.1](image/38.png){#fig:001 width=70%}

Отмечены основные условия для криптографической хэш-функции (рис. [-@fig:002]).

![Вопрос 4.1.2](image/39.png){#fig:002 width=70%}

Отмечены алгоритмы цифровой подписи (рис. [-@fig:003]).

![Вопрос 4.1.3](image/40.png){#fig:003 width=70%}

В информационной безопасности аутентификация сообщения или аутентификация источника данных-это свойство, которое гарантирует, что сообщение не было изменено во время передачи (целостность данных) и что принимающая сторона может проверить источник сообщения (рис. [-@fig:004])

![Вопрос 4.1.4](image/41.png){#fig:004 width=70%}

Определение обмена ключами Диффи-Хэллмана. (рис. [-@fig:005]).

![Вопрос 4.1.5](image/42.png){#fig:005 width=70%}

## Цифровая подпись

По определению цифровой подписи протокол ЭЦП относится к протоколам с публичным ключом (рис. [-@fig:006]).

![Вопрос 4.2.1](image/43.png){#fig:006 width=70%}

лгоритм верификации электронной подписи состоит в следующем. На первом этапе получатель сообщения строит собственный вариант хэш-функции подписанного документа. На втором этапе происходит расшифровка хэш-функции, содержащейся в сообщении с помощью открытого ключа отправителя. На третьем этапе производится сравнение двух хэш- функций. Их совпадение гарантирует одновременно подлинность содержимого документа и его авторства (рис. [-@fig:007]).

![Вопрос 4.2.2](image/44.png){#fig:007 width=70%}

Электронная подпись обеспечивает все указанное, кроме конфиденциальности (рис. [-@fig:008]).

![Вопрос 4.2.3](image/45.png){#fig:008 width=70%}

Для отправки налоговой отчетности в ФНС используется усиленная квалифицированная электронная подпись (рис. [-@fig:009]).

![Вопрос 4.2.4](image/46.png){#fig:009 width=70%}

Верный ответ укзаан на изображении (рис. [-@fig:010]).

![Вопрос 4.2.5](image/47.png){#fig:010 width=70%}

## Электронные платежи

Известные платежные системы - Visa, MasterCard, МИР (рис. [-@fig:011]).

![Вопрос 4.3.1](image/48.png){#fig:011 width=70%}

Верный ответ на изображении (рис. [-@fig:012]).

![Вопрос 4.3.2](image/49.png){#fig:012 width=70%}

При онлайн платежах используется многофакторная аутентификация (рис. [-@fig:013]).

![Вопрос 4.3.3](image/50.png){#fig:013 width=70%}

## Блокчейн

Proof-of-Work, или PoW, (доказательство выполнения работы) — это алгоритм достижения консенсуса в блокчейне; он используется для подтверждения транзакций и создания новых блоков. С помощью PoW майнеры конкурируют друг с другом за завершение транзакций в сети и за вознаграждение.
Пользователи сети отправляют друг другу цифровые токены, после чего все транзакции собираются в блоки и записываются в распределенный реестр, то есть в блокчейн.  (рис. [-@fig:014]).

![Вопрос 4.4.1](image/51.png){#fig:014 width=70%}

Консенсус блокчейна — это процедура, в ходе которой участники сети достигают согласия о текущем состоянии данных в сети. Благодаря этому алгоритмы консенсуса устанавливают надежность и доверие к самоу сети. (рис. [-@fig:015]).

![Вопрос 4.4.2](image/52.png){#fig:015 width=70%}

Ответ - цифровая подпись (рис. [-@fig:016]).

![Вопрос 4.4.3](image/53.png){#fig:016 width=70%}

# Выводы
 Я прошла третий блок и завершила внешний курс по информационной безопасности
