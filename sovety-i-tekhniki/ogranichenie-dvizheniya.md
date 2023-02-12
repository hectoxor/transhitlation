# Ограничение движения

## Основы ограничения движения

Для достижения целей роботам необходимо движение; руки должны поворачиваться, колеса - вращаться и т. д. Однако движение, не связанное непосредственно с этими действиями, может повлиять на точность и аккуратность механизмов робота. Это непреднамеренное движение должно быть надлежащим образом ограничено, или **сдержано**.

Длинные и тонкие конструкции могут изгибаться и деформироваться, что затрудняет взаимодействие с объектами и повторяемость операций. Используйте кронштейны и дополнительные [экструзии](https://www.revrobotics.com/ftc/structure/extrusion/) или [С-каналы](https://www.revrobotics.com/ftc/structure/channel/) для **укрепления** и ограничения таких конструкций.

## Как ограничивать движение

Шестерни и звездочки должны быть выровнены, иначе они не будут работать должным образом.

{% hint style="danger" %}
Если две звездочки не будут идеально выровнены друг относительно друга, цепь между ними будет сходить со звездочек.
{% endhint %}

Выравнивание деталей на валу и предотвращение соскальзывания самого вала очень важно для надежной работы роботизированных механизмов. Для выравнивания и фиксации этих деталей используйте комбинацию распорок(спейсеров) и хомутов вала.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M7xZrfXp93Fnloi8g1R%2F-M7xgaxdf9RgjLOtNorx%2FThree%20Spacers%20Chart.png?alt=media&#x26;token=d56e0bfe-a930-4214-bf5d-3cd83d84f201" alt=""><figcaption></figcaption></figure>

## Конструирование стыков

Еще одним важным элементом для правильного ограничения движения является конструкция соединений. Места соединения структурных компонентов, таких как экструзия и канал, должны быть надлежащим образом поддержаны, чтобы избежать разрушения структуры во время движения.

### Закрепите с помощью 2 или более кронштейнов

В большинстве случаев стыки должны иметь как минимум две стороны, соединенные скобами для прочности и устойчивости. Это особенно актуально для пластиковых скоб. Обычно для этого берут два одинаковых вида кронштейна и соединяют их между собой, но это могут быть и два разных вида кронштейнов, например, кронштейн 90 градусов ([REV-41-1305](https://www.revrobotics.com/15mm-Plastic-Brackets/))([REV-41-1480](https://www.revrobotics.com/15mm-Metal-Brackets/)) и кронштейн внутреннего угла ([REV-41-1320](https://www.revrobotics.com/rev-41-1320-pk8/))([REV-41-1479](https://www.revrobotics.com/rev-41-1479-pk8/)), установленные на одном углу.

&#x20;****&#x20;

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlBl-KdeMsqjyFTh34y%2F-MlBteXzWZEYjnRtp-NG%2Fdouble%20up%20bracket.png?alt=media&#x26;token=afa79f5e-6885-40d3-aa4b-fdfa98a563c2" alt=""><figcaption></figcaption></figure>

### Используйте конические экструзии ****&#x20;

При использовании скоб для соединения экструзии, соединение будет намного прочнее, если конец экструзии будет скошен (срезан под углом) так, чтобы конец был вплотную с поверхностью прилегающей экструзии.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlBl-KdeMsqjyFTh34y%2F-MlBu-9QamQcRqfrMaZw%2Fbeveled%20extrusion%20joint.png?alt=media&#x26;token=e537fe26-68ec-42d3-b59d-aaf1e097201c" alt=""><figcaption></figcaption></figure>

Различные углы наклона кронштейнов можно комбинировать для создания конструкций. В этом примере все соединения скошены, чтобы прилегать к прилегающему экструзии вплотную.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlBl-KdeMsqjyFTh34y%2F-MlBu9LE25g-rel_sN5R%2Fdifferent%20angle%20brackets.png?alt=media&#x26;token=bd72f2a5-602b-4dc7-a094-2cf14a23af25" alt=""><figcaption></figcaption></figure>

### Способы создания соединений под углом в 90 градусов

Существует три основных способа создания соединений экструзии под углом 90°. Наиболее распространенным является кронштейн 90°, который соединяет части экструзии под углом 90° в одной плоскости. Второй тип - кронштейн для внутренних углов - функционально эквивалентен кронштейну 90°. Третий тип называется кронштейном для соединения внахлестку, который позволяет двум частям экструзии "накладываться друг на друга".

**90° кронштейн**

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlBl-KdeMsqjyFTh34y%2F-MlBtYVQmzLIEl1laVmD%2F90%20degree%20bracket%20%20REV-41-1305.png?alt=media&#x26;token=8e1daa2f-df33-4ef4-8038-293916a31863" alt=""><figcaption></figcaption></figure>

**Кронштейн внутреннего угла**

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlBl-KdeMsqjyFTh34y%2F-MlBtU6x7khT7umhDJt6%2Finside%20corner%20bracket%20REV-41-1320.png?alt=media&#x26;token=21ebb14e-2609-4dcc-95a6-dbc5150e05c7" alt=""><figcaption></figcaption></figure>

**Угловой кронштейн с нахлестом** ([REV-41-1321](https://www.revrobotics.com/rev-41-1321/))

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlBl-KdeMsqjyFTh34y%2F-MlBtQ2D5bz8zJjaDYG2%2Flap%20corner%20bracket%20REV-41-1321.png?alt=media&#x26;token=28a57cfd-4375-4ba7-8d34-dab2c3c73508" alt=""><figcaption></figcaption></figure>
