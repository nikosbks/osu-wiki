Точность
=========

Точность (Accuracy) — мера того, насколько хорошо игрок попадает в ритм карты.

Подробности
-------------

В зависимости от контекста, под точностью могут пониматься немного разные вещи. Во-первых, можно говорить о точности прохождения карты, на которую влияют:

-   [Параметр OD](/wiki/Beatmap_Editor/Song_Setup) сыгранной карты;
-   Активированные моды [Easy](/wiki/Difficulties/osu!/Easy) или [Hardrock](/wiki/Game_Modifiers).

С самими же игроками связано две точности:

-   Общая (overall) точность. Она складывается из всех когда-либо выбитых нот по следующему правилу (перевод описания с сайта): «Точность вычисляется как среднее значение между точностями всех когда-либо отправленных Вами результатов, причём каждая сложность считается отдельно. Расчёт основан на ценности каждой выбитой ноты: 50 — это 1/6 от 300 (идеальный удар), а промах — это 0».

Данный параметр убран с сайта, и увидеть его можно только на экране результатов, если прокрутить вниз.

-   [PP](/wiki/Performance_Points)-точность. Она считается почти так же, как общая, но в расчётах участвует ещё и количество PP, полученное за каждую карту: чем больше PP у результата, тем сильней он влияет на точность. Таким образом, как и при расчёте игрового ранка, на PP-точность влияют только 100 лучших рекордов; всё, что находится ниже, имеет вес, близкий к нулю.

Формулы расчёта точности
---------------------------

### Стандарт

Точность — сумма точностей всех ударов, делённая на максимально возможную сумму. Другими словами:

**Точность = Точность всех ударов / (Число всех ударов × 300)**

| Точность всех ударов | Число всех ударов |
| -------------------- | ----------------- |
| (число "50" × 50 + число "100" × 100 + число "300" × 300) | (Число промахов + число "50" + число "100" + число "300") |

### Тайко

Точность — сумма точностей всех ударов, делённая на число нот (драмроллы и спиннеры не участвуют в расчёте). Точности ударов:

-   GREAT (良) = 100%;
-   GOOD (可) = 50% (половина);
-   MISS/BAD (不可) = 0% (сброс комбо);

**Точность = Точность всех ударов / (Число нот × 300)**

| Точность всех ударов | Число нот |
| -------------------- | --------- |
| (Число "100" × 0.5 + число "300" × 1) × 300 | (Число промахов + число "100" + число "300") |

### Catch the Beat

Точность — число пойманных фруктов, делённое на число всех фруктов. Спиннеры в расчёте не участвуют, а все фрукты (даже маленькие капельки) «стоят» одинаково.

**Точность = Число пойманных фруктов / Число всех фруктов**

| Условия |
| ----------- |
| Бананы (фрукты на спиннерах) не считаются |

### Мания

Точность считается почти так же, как и в стандарте.

**Точность = Точность всех ударов / (Число ударов × 300)**

| Точность всех ударов | Число всех ударов |
| -------------------- | ----------------- |
| (Число "50" × 50 + число "100" × 100 + число "200" × 200 + число "300" × 300 + число "MAX" × 300) | (Число промахов + число "50" + число "100" + число "200" + число "300" + число "MAX") |

Как можно заметить, "MAX" и "300" оказывают одинаковое влияние на точность, несмотря на то, что "MAX" сильней влияет на число очков.

Показатели точности
--------------------

### Экран результатов

#### Ранкинг


Оценка за прохождение, число ударов каждого типа и процент точности. Подробности можно узнать в [этой статье](/wiki/Score).

![Пример для стандарта](Accuracy_osu!_Small.jpg "Пример для стандарта") ![Пример для тайко](Accuracy_Taiko_Small.jpg "Пример для тайко")
![Пример для Catch the Beat](Accuracy_CtB_Small.jpg "osu!Пример для Catch the Beat") ![Пример для osu!Mania](Accuracy_Mania_Small.jpg "Пример для osu!Mania")

#### График производительности


График Вашей игровой производительности на протяжении игры. Для дополнительной информации наведите на него курсор:

![График производительности](Accuracy_TR.jpg "График производительности")

##### Точность

| Term | Meaning |
| ---- | ------- |
| Погрешность | **Эти два числа показывают, насколько В СРЕДНЕМ Ваши нажатия происходили раньше и позже.** Чем выше [OD](/wiki/Beatmap_Editor/Song_Setup) карты, которую Вы играете, тем меньше должны быть эти значения. Они являются [математическими ожиданиями](//en.wikipedia.org/wiki/ru:%D0%9C%D0%B0%D1%82%D0%B5%D0%BC%D0%B0%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%BE%D0%B5_%D0%BE%D0%B6%D0%B8%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5) ранних и поздних нажатий соответственно. |
| Разброс (Unstable Rate) | **Это значение показывает, насколько РАВНОМЕРНО Вы нажимаете на ноты.** Чем ниже, тем лучше (у топ-игроков это значение очень часто не превышает 100). Обратите внимание: измеряется равномерность нажатий, но не точность; равномерно нажимать можно как вовремя, так и слишком рано/поздно. Данный показатель — [среднеквадратическое отклонение](//en.wikipedia.org/wiki/ru:%D0%A1%D1%80%D0%B5%D0%B4%D0%BD%D0%B5%D0%BA%D0%B2%D0%B0%D0%B4%D1%80%D0%B0%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%BE%D0%B5_%D0%BE%D1%82%D0%BA%D0%BB%D0%BE%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5) всех нажатий в миллисекундах, умноженное на 10. |

##### Спин [только для стандарта]

| Term | Meaning |
| ---- | ------- |
| Скорость (Speed) | **Средняя скорость вращения всех спиннеров на карте.** Max — максимальное значение RPM (revolutions per minute, обороты/мин.) по всем спиннерам. |
| Разброс (Unstable Rate) | **Значение, основанное на соотношении максимальной и средней скоростей**, чем ниже, тем лучше. Формула неизвестна, но предполагается, что она похожа на формулу разброса нажатий для точности. |

**Примечания:**

-   Описанные выше значения можно увидеть только после просмотра реплея, после чего они исчезают.
-   В связи с тем, как реализована работа игровых модов, погрешность и разброс умножаются на скорость песни. Таким образом, для реплеев с [Double Time](/wiki/Game_Modifiers) результаты нужно разделить на 3/2. Аналогично, при игре с [Hardrock](/wiki/Game_Modifiers) их нужно умножить на 4/3.
