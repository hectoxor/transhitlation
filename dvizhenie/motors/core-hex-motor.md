---
описание: Core Hex Motor Basics
---

# Core Hex Motor

Core Hex Motor ([REV-41-1300](https://www.revrobotics.com/rev-41-1300/)) - это мотор, который имеет ориентацию 90 градусов и выходной вал с внутренней резьбой для максимальной гибкости и простоты использования. Вставьте любой из стандартных [5 мм шестигранных валов REV](https://www.revrobotics.com/ftc/motion/bearings-linear-slides-pillow-blocks/) в Core Hex Motor или через него для создания выходных валов двигателя нестандартной длины. Core Hex Motor имеет встроенный магнитный квадратурный энкодер, совместимый с устройствами с логическим уровнем 5 В или 3,3 В, включая концентратор управления ([REV-31-1595](https://www.revrobotics.com/rev-31-1595/)) и концентратор расширения ([REV-31-1153](https://www.revrobotics.com/rev-31-1153/)). &#x20;

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M8MarlMx5meMXBAcMX_%2F-M8Mau1m3YkY8a8rLOaT%2Fimage. png?alt=media&#x26;token=1f0ffc5b-afed-479c-876d-f95974a111a1" alt=""><figcaption></figcaption></figure>

### Распиновка

Core Hex Motor использует 2-контактный разъем JST-VH для питания двигателя и 4-контактный JST-PH для обратной связи со встроенным энкодером. Более подробную информацию об использовании кабелей и разъемов, входящих в комплект Core Hex Motor, см. в [REV Control System - Cable and Connectors documentation](https://docs.revrobotics.com/duo-control/control-system-overview/cables-and-connectors). На рисунке ниже показана распиновка разъемов питания двигателя и энкодера.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M_M8cPZpdT88Tye8xPn%2F-M_MCcUszaBq8eeo9Rmp%2FHD%20Hex%20Motor_Encoder%20Pinout1_Export. svg?alt=media&#x26;token=b7cf4b6d-d8aa-407c-bf6d-609253e815cf" alt=""><figcaption></figcaption></figure>

### Характеристики продукта

* Выходной вал: 5 мм внутренний шестигранник
* Вес: 7 унций
* Напряжение: 12 В постоянного тока
* Свободная скорость: 125 об/мин
* Крутящий момент при остановке: 3,2 Н-м
* Ток остановки: 4,4 А
* Передаточное число: 72:1
* Количество отсчетов энкодера на оборот
  * На двигателе - 4 отсчета/об.
  * На выходе - 288 отсчетов/об.

## Когда использовать?

Общая рекомендация - использовать двигатель Core Hex для более легких манипуляторов и вводов.&#x20;

{% hint style="info" %}
Посетите страницу [_Выбор и привод_](broken-reference), чтобы узнать больше о том, как определить, какой тип привода подходит для вашего механизма._
{% endhint %}

## Как использовать?

{% hint style="info" %}
Чтобы узнать больше о встроенных энкодерах и проводке для шестигранного двигателя, посетите руководство по системе управления.
{% endhint %}

### Как установить шестигранный двигатель&#x20;

Двигатель Core Hex Motor имеет две грани для монтажа с двух сторон двигателя. Комбинация шаблонов движения выставляется под разными углами на каждой грани, что дает двенадцать различных углов наклона двигателя. На изображениях ниже показана базовая структура монтажа для двух из двенадцати доступных положений.&#x20;

{% hint style="warning" %}
На изображениях показана базовая система крепления. Всегда рекомендуется должным образом поддерживать элементы вашего робота с помощью более 2 или более пластиковых кронштейнов&#x20;
{% endhint %}

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M8vmWNQpIfKGFT4hhI0%2F-M8w-OcpkhH60EeMi9iI%2FScreenshot%20(46). png?alt=media&#x26;token=499e490b-7dec-4b42-b51e-f003582fb83e" alt=""><figcaption></figcaption></figure>
