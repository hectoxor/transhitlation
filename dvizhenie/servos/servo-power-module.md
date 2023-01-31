# Модуль питания сервопривода

## Основы модуля питания сервопривода

REV Servo Power Module ([REV-11-1144](https://www.revrobotics.com/rev-11-1144/)) - это инжектор питания 6 В 90 Вт, который позволяет использовать мощные RC-сервоприводы в приложениях, где контроллер робота не может обеспечить достаточную мощность.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8VuTXTeaMyPtvVrNSd%2F-M8WMcrnMWEB7n-inTqu%2F2.png?generation=1590771487323342&#x26;alt=media" alt=""><figcaption></figcaption></figure>.

### Технические характеристики продукта

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FH9K1InCLC1ZxIkdPJt31%2Fuploads%2FyiWxbuAKk1gmi9N16RaR%2Fspm%20labeled.png?alt=media&#x26;token=b436763e-86a1-430a-a811-970f6114c5c6" alt=""><figcaption></figcaption></figure>

| Ключевые термины | Ключевые метрики |
| ---------------------------------------------------------------------------------------------- | -------------------- |
| **Номинальное входное напряжение** | 12 В | |
| **Диапазон рабочего напряжения** | 7,0 В - 20 В | |
| **Минимальное напряжение при запуске** | 9,0 В | |
| **Выходное напряжение** | 6 В | |
| **Количество каналов** | 6 | |
| <p><strong>Max. Total Output Current</strong></p><p><strong>(across all Channels)</strong></p> | 15A |
| **Max. Total Output Power** | 90W |
| **Size** | 3.6” x 1.52” x 0.81” |
| **Weight** | 2.0oz/57g |

## How to Use&#x20;

### Electrical Connections

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8VuTXTeaMyPtvVrNSd%2F-M8WMcrpi_Pd87PP76iS%2F4.png?generation=1590771487272705&#x26;alt=media" alt=""><figcaption></figcaption></figure>

The Servo Power Module has two screw terminals for 12V power input. It is recommended to use ring or fork terminals designed for #6 or M3 screw terminals.

Using an appropriate wire gauge, 18 AWG or larger, tightly crimp either a ring or fork terminal on the wire. Insert the crimped terminal into the screw terminal and tighten the screw.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8VuTXTeaMyPtvVrNSd%2F-M8WMcrqMsXUzLIElogM%2F5.png?generation=1590771487662184&#x26;alt=media" alt=""><figcaption></figcaption></figure>

The input and output channels accept standard 3-wire 0.1” pitch servo/PWM cables. Please refer to the figure above or the case markings for proper orientation.

### Светодиодные индикаторы состояния

Каждый канал имеет соответствующий светодиодный индикатор состояния, который показывает состояние подключенного ШИМ-сигнала. В таблице ниже описано соответствующее состояние каждого светодиода.

| **Состояние** | **Паттерн** | **Состояние**.
| --------------------- | -------------- |
| Нет сигнала | Мигающий янтарный |
| Левый/реверсивный сигнал | Постоянный красный |
| Центр/нейтральный сигнал | Постоянно горит янтарным |
| Сигнал вправо/вперед | Постоянный зеленый |

### Отключение при перегрузке по току&#x20;

Если модуль питания сервопривода обнаруживает общий выходной ток более 15 А, он переходит в режим отключения, в котором выход 6 В отключается до устранения перегрузки по току. В режиме отключения синий светодиод питания выключается, тускнеет или мерцает, указывая на то, что состояние перегрузки по току все еще присутствует.

В случае частых отключений по току убедитесь, что общий ток срабатывания всех подключенных сервоприводов не превышает 15 А.
