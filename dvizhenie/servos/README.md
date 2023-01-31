---
description: Основы сервоприводов
---

# Сервоприводы

Серводвигатели - это специализированный вид двигателей, которыми можно управлять для перемещения на определенный угол, а не для непрерывного вращения, как двигателями постоянного тока. Вместо шестигранного выходного вала, как у двигателя постоянного тока, сервоприводы имеют выходной шлиц. Шлиц - это специальная канавка, вырезанная на валу, которая позволяет передавать вращение серводвигателя на прикрепленный алюминиевый сервопривод ([REV-41-1363](https://www.revrobotics.com/rev-41-1363/)) или [адаптер для серво](https://www.revrobotics.com/ftc/motion/wheels-hubs-adapters/).Шлицы подобны ключам, поэтому только подходящие типы подходят друг к другу. Все сервоприводы REV Robotics используют шлицы 25T. Если шестерни или шлицы сервопривода REV Robotics Smart Robot Servo ([REV-41-1097](https://www.revrobotics.com/rev-41-1097/))если они повреждены, их можно заменить с помощью сменного комплекта шестерен([REV-41-1168](https://www.revrobotics.com/rev-41-1168/)).&#x20;

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FH9K1InCLC1ZxIkdPJt31%2Fuploads%2FQQWfPA2jvlDUhJOiFNuW%2FREV-41-1097%20SRS%20drawing.png?alt=media&#x26;token=f0e899ab-11df-4aa2-bb64-7eb02273adef" alt=""><figcaption></figcaption></figure>

Обычные серводвигатели принимают запрограммированный диапазон входного сигнала и преобразуют его в угловой диапазон. Например, для сервопривода с диапазоном 270°, если диапазон входного сигнала от 0 до 1, то при подаче сигнала 0 сервопривод повернется в точку -135°. При подаче сигнала 1 сервопривод повернется на +135°. Входы между минимальным и максимальным значением имеют соответствующие углы, равномерно распределенные между минимальным и максимальным углом сервопривода.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MB_vrFI_mJbhAOGXIO5%2F-MB_yzhf7dnGkYfx6zkp%2FServo_270_Range_Full_Green-01.png?alt=media&#x26;token=db791fac-0f86-42d8-9651-1c0e42ae87ad" alt=""><figcaption></figcaption></figure>

### Серво адаптеры

Сервоадаптеры REV Robotics подходят для сервоприводов со шлицем 25T, таких как REV Robotics Smart Robot Servo. В дополнение к разнообразным рожкам для сервоприводов, которые поставляются с сервоприводом Smart Robot Servo, есть еще четыре пользовательских сервоадаптера, которые упрощают использование сервоприводов с REV 15mm Building System.

**Servo Gear Adapters** convert a 25T servo into 15 tooth Delrin gear which is compatible with the other REV Robotics Plastic Gears.&#x20;

**Servo Shaft Adapters** convert a 25T spline servo output shaft into a female 5mm hex socket.  This adapter can be used to drive a hex shaft directly.

**Aluminum Servo Horns** have a tapped hole pattern that can be directly mounted to any of the REV Robotics gears, wheels, or sprockets with the Motion Pattern.

**Aluminum Double Servo Arms** ([REV-41-1820](https://www.revrobotics.com/rev-41-1820/)) **** have two tapped holes that can be directly mounted to any of the REV Robotics extrusion, channel, or brackets.&#x20;

## Servos with the Control Hub and Expansion Hub

Teams should be aware of the number of servo motors they attach to each Hub. The Control Hub ([REV-31-1595](https://www.revrobotics.com/rev-31-1595/)) and Expansion Hub ([REV-31-1153](https://www.revrobotics.com/rev-31-1153/)) only can handle 5 Amps through all 6 servo ports. The maximum current a servo will draw is 2.0 Amps, called the stall current. A servo will draw the stall current when it is applying the maximum force, but it is not moving. For example, a servo can stall when a mechanism needs to hold something or a heavy object blocked the path of the servo motion.&#x20;

Normally servos do not draw the maximum current, but teams do not know what might happen during matches. To protect against overdrawing the current on the Hub, only attach 2 servos to a Control Hub or Expansion Hub. Teams can safely use 4 servos: 2 servos on the Control Hub and 2 servos on the Expansion Hub.

If more power is required, consider using the REV Servo Power Module ([REV-11-1144](https://www.revrobotics.com/rev-11-1144/)). It is a 6V 90W power injector that enables the use of high-power RC servos in applications where a robot controller cannot provide adequate power.
