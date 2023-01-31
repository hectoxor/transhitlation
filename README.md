# Введение в Структуру

### Основы Структуры&#x20;

REV DUO Build System имеет два главных структурных компонента, [Extrusion](https://www.revrobotics.com/ftc/structure/15mm-extrusion/) и [Channel](https://www.revrobotics.com/competition/ftc/structure/channel/).  REV Extrusion это прямоугольная структурная рельса с пазами для изделий формата [M3 ](https://www.revrobotics.com/ftc/hardware/fasteners/)на всех четырех сторонах. Пазы в Extrusion позволяют устанавливать кронштейны и другие предметы в любое положение на рельсе. REV Channel это более крупный структурный компонент, позволяющий установку приводов, кронштейнов и других элементов на установленных интервалах. REV Channel представляет собой комбинацию **системы с фиксированным шагом** (известную как **Extended Motion Pattern**) и **системы extrusion** для гибкости дизайна.

Все структурные компоненты REV DUO совместимы с форматом M3.

### Система Extrusion и Система с фиксированным шагом

15-и миллиметровая система extrusion обеспечивает более гибкий, итеративный процесс работы чем системы с фиксированным шагом. **Системы с фиксированным шагом** имеют определенный шаблон отверстий для установки деталей; все устанавливаемые детали расположены на расстоянии, кратном фиксированному шагу или установленной доле фиксированного шага.

По сравнению, система extrusion позволяет гибко устанавливать монтажные позиции вдоль пазов. Просто вставьте любые кронштейны или детали, которые необходимо установить, в соответствующий паз и отрегулируйте их до нужного положения.

Мы убеждены, что чем проще вносить изменения в дизайн, тем проще его улучшать.

Ознакомьтесь со страницами ниже чтобы узнать больше о компонентах REV DUO.

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

### Extended Motion Pattern&#x20;

В отличии от 15-и миллиметровой Extrusion, прочие компоненты REV DUO имеют фиксированный шаг. [Structural brackets](broken-reference) have M3 holes on an 8mm pitch. While [Motion Brackets](broken-reference) have the Motion Pattern, a circular M3 hole pattern on a 16mm diameter is used to mount to REV Robotics shaft accessories.&#x20;

Канал C, канал U и плоская пластина имеют расширенную схему движения, модифицированную схему движения с круглым отверстием M3 на диаметре 32 мм. Это повторяется по всей длине канала для установки подшипников, валов, кронштейнов и т. д.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FH9K1InCLC1ZxIkdPJt31%2Fuploads%2FkgmGYol4aZrcqSC8WltV%2FScreenshot%202022-05-27%20135659.png?alt=media&#x26;token=b0fb2b2e-a4dc-48f7-a359-fb7d53c115e7" alt=""><figcaption></figcaption></figure>

Расширенный шаблон движения начинается с отверстий M3 с шагом 8 мм по центру канала. Каждое из отверстий на шаге центральной линии образует «основу» для равностороннего треугольника со сторонами 8 мм, который простирается наружу к краям канала. Через каждые 16 мм открывается центральное отверстие, которое становится гнездом для подшипника диаметром 9 мм для крепления валов и подшипников.
