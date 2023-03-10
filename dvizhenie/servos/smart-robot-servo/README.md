---
description: SRS Basics
---

# Smart Robot Servo

REV Robotics Smart Robot Servo (SRS) ([REV-41-1097](https://www.revrobotics.com/rev-41-1097/)) это конфигурируемый сервопривод с металлическими зубчатыми колесами, который устраняет необходимость в выравнивании и регулировке механизмов на основе сервопривода. Один SRS может использоваться как стандартный угловой сервопривод, пользовательский угловой сервопривод и сервопривод непрерывного вращения путем простого изменения настроек.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M95GquH9Q5xxbGh4P4K%2F-M95GvywvJjRnMyKX-5f%2FAA_Smart_Robot_Servo_Single.png?alt=media&#x26;token=719199e1-3ba3-4319-b564-a2521792bcde" alt=""><figcaption></figcaption></figure>

### Технические характеристики продукта&#x20;

REV Robotics Smart Robot Servo включает в себя следующие функции:

* Работа по умолчанию
  * Движение на 270° при полном диапазоне входных импульсов
*   Металлические шестерни


* Интеллектуальные функции
  * Программируется с помощью программатора REV SRS([REV-31-1108](https://www.revrobotics.com/rev-31-1108/))
  * Предельный режим сервопривода
    * Установка правого и левого угловых пределов
      * SRS не будет двигаться дальше пределов
* Непрерывный режим
  * SRS вращается непрерывно
  * Скорость и направление задаются входным импульсом

### Механические характеристики&#x20;

|                                            |                          |
| ------------------------------------------ | ------------------------ |
| **Крутящий момент при остановке (при 6V)** | 13.5 kg-cm / 187.8 oz-in |
| **Скорость (при 6V)**                      | 0.13s/60º                |
| Максимальный угловой диапазон              | 270º                     |
| **Материал шестерни**                      | Brass                    |
| **Тип шлица**                              | 25T                      |
| Размеры                                    | 40.2mm x 20.0mm x 38.0mm |
| **Вес**                                    | 2.05oz.                  |

### Электрические характеристики

|                            | Min  | Nominal  | Max  |
| -------------------------- | ---- | -------- | ---- |
| **Номинальное напряжение** | 4.8V | 6.0V     | 7.4V |
| **Ток задержки (at 6V)**   |      |          | 2.0A |

Входной импульс:

* Мин: 500 мкс
* Центр: 1500 мкс
* Макс: 2500 мкс

### Содержание набора:&#x20;

В комплект поставки REV Robotics SRS входит следующее:

* REV Smart Robot Servo
* Ассортимент рожков сервопривода (рычагов)
* Крепеж для монтажа серворуля

{% hint style="info" %}
Является ли сервопривод подходящим приводом для вашего механизма? См. __ Раздел "[Выбор привода](../../vybor-privoda.md)", чтобы узнать больше_._
{% endhint %}

## Режимы работы

Из коробки SRS работает как сервопривод с углом поворота 270°. Однако программатор REV SRS может перенастроить SRS, чтобы установить угловые ограничения или переключить его в режим непрерывного вращения.

{% hint style="info" %}
Для получения дополнительной информации о том, как использовать программатор SRS для изменения режимов сервопривода, см. раздел [Программатор SRS](../srs-programmer.md)
{% endhint %}

### Обычный режим&#x20;

Диапазон по умолчанию для SRS составляет 270°. Этот диапазон сопоставлен с диапазоном входных импульсов от 500 мкс до 2500 мкс с 1500 мкс в качестве центральной точки. На рисунке ниже описана зависимость импульса от угла.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MB_vrFI_mJbhAOGXIO5%2F-MB_yzhf7dnGkYfx6zkp%2FServo_270_Range_Full_Green-01.png?alt=media&#x26;token=db791fac-0f86-42d8-9651-1c0e42ae87ad" alt=""><figcaption></figcaption></figure>

### Непрерывное вращение&#x20;

SRS может быть настроен с помощью программатора SRS для работы в режиме непрерывного вращения. В этом режиме один и тот же диапазон входных импульсов сопоставляется с направлением и скоростью. В приведенной ниже таблице перечислено отображение импульсов для направления и скорости.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M8WQp_aU3jlfmzyZA5V%2F-M8WUtfWcre4DktYBnv0%2FScreenshot%20(13).png?alt=media&#x26;token=0483c54f-8ec2-4be0-a3e8-b5dd3374655a" alt=""><figcaption></figcaption></figure>

### Угловые пределы

SRS может быть легко настроена с помощью программатора SRS для ограничения движения вправо и влево под двумя заданными пользователем углами. Входные импульсы, проходящие мимо пределов, будут игнорироваться, и SRS будет удерживать предельный угол. Любые два угла могут быть установлены в качестве предельных при условии, что левый предел находится слева от центральной мертвой зоны, а правый - справа от центральной мертвой зоны. В таблице ниже показаны допустимые области для левого и правого пределов.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MB_vrFI_mJbhAOGXIO5%2F-MB_z21vt7t6VYO6gk0T%2FServo_270_Range_Limit_Too_Close.png?alt=media&#x26;token=05207ceb-7734-400f-9423-eed9fd439aab" alt=""><figcaption></figcaption></figure>

После программирования допустимых пределов SRS будет игнорировать любые импульсы, превышающие пределы, и удерживать предельный угол. Например, на рисунке ниже показано, что произойдет, если установить левый предел -30° и правый предел +60°.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MB_vrFI_mJbhAOGXIO5%2F-MB_z3iQG92g4sFKXPuk%2FServo_Full_270_Range_And_Limits-01.png?alt=media&#x26;token=b86e324d-b901-48dc-af88-fca499bb04f7" alt=""><figcaption></figcaption></figure>
