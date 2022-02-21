---
fontfamily: tnr
# pointsize: 10pt
# lineheight: 12pt
bibliography: /home/volk/Library/bibtex/lib.bib
title: Cu(Fe,Co)/h-BN nanohybrids for CO oxidation
author: Ilia Volkov
csl: /home/volk/Documents/Work/gost-csl/GOST-styles-for-Zotero/gost-r-7-0-5-2008-num-appear.csl
# papersize: a4
plot-configuration: /home/volk/.config/pandoc-plot/config.yaml
---

# Приготовление смеси для

Чистое железо на нитриде бора было приготовлено методом восстановления в растворе абсолютизированного этанола в ледяной бане. В качестве реагентов использовались хлорид железа 2 и тетраборат натрия.

$FeCl_2 * H_2O$

```{.run cmd="python" in="script" out="text"}
from chempy import balance_stoichiometry
reac, prod = balance_stoichiometry({'NaBH4', 'FeCl2:4H2O'}, {'Fe', 'NaCl', 'BH3', 'H2', H2O})
from pprint import pprint
pprint(dict(reac))
 ```


Методика взята из сатьи [Synthesis of bimetallic Fe–Zn nanoparticles and its application towardsadsorptive removal of carcinogenic dye malachite green and Congo redin water]

Для приготовления смеси была разработана следующая методика:

Деоксидировать воду протоком N2 в течение 30 минут, затем добавить 0.1 М FeCl3*6H2O в 100 мл этанол/воды (30/70, v/v). В протоке азота добавили 0.3 М NaBH4 (количество не ясно) и перемешивалось 10 минут до полявления черного цвета. Черные частицы были отделены магнитом. Все отмывалось деоксидированной водой и ацетоном.

2Fe + 2H2O + BH4 -> Fe + BO2 +4H + H2

Цинк был добавлен в отмытый раствор наночастиц железа в виде 0.1 M Zn(NO3)2*6H2O в 50 мл этанола. Перемешивали 30 минут.

Fe(s) + Zn2+ -> Fe2+ + Zn(s)

Затем все высушивалось в воздухе 120 градусов в течение 24 ч

План эксперимента:

Синтез наночастиц FeZn/h-BN двумя методами:
1. Раздельный метод (описан выше)
2. Метод соосаждения (Смесь растворов FeCl3 + ZnNO3? (может быть нужен будет хлорид))

Рассчет реагентов

Eth - 10 ml
H2O - 90 ml
h-BN - 100 mg
FeCl2*4H2O - 34 mg
Zn(NO3)2*6H2O - 4.6 mg
NaBH4 - 21.25 mg

Приготовил 50 мл суспензии (3 мин 40% уз), добавил раствор NaNO3 (460 мкл),  и засыпал хлорид железа, еще раз проультразвучил (3 минуты). Поставил суспензию и воду в вакуум для дегазации. NaBH4 начал добавлять по каплям 1мл через инфузионный насос,  но он отказывается работат (газ в системе и кнопки не работают). В итоге долил быстро 9 мл из шприца. Отмывал 2 раза, 1 раз просто сепарировал, 1 раз этанолом.
