---
description: Motor Basics
---

# Motors

Electric motors are the core power plant of most robots. There are two types of motors in the REV DUO Build System: the Core Hex Motor ([REV-41-1300](https://www.revrobotics.com/rev-41-1300/)) and the HD Hex Motor ([REV-41-1301](https://www.revrobotics.com/rev-41-1301/)). Both motors are brushed DC motors. The image below showcases the common elements of a bushed DC motor.&#x20;

#### Elements of a Brushed DC Motor

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8MarlMx5meMXBAcMX_%2F-M8MhYlMn7b3u0xtE-Zr%2F1.png?generation=1590609462403887&#x26;alt=media" alt=""><figcaption></figcaption></figure>

Brushed DC motors without a gear box can be estimated to be \~80% efficient, meaning if a motor is drawing 60 watts of power \~48 watts will be turned into mechanical energy and \~12 watts will become heat. Once a gear box is added the overall efficiency of the system goes down.

### Key Metrics&#x20;

DC brushed motors can be described by some key metrics:

{% tabs %}
{% tab title="Stall Torque" %}
**Stall Torque** is measured when the motors RPM is zero and the motor is drawing its full **Stall Current**. This value is the maximum torque the motor is ever capable of outputting. Keep in mind the motor is not capable of outputting this torque for an indefinite period of time. Waste energy will be released into the motor as heat. When the motor is producing more waste heat than the motor body is capable of dissipating the motor will eventually overheat and fail.
{% endtab %}

{% tab title="Stall Current" %}
**Stall Current** is the maximum amount of current the motor will draw. The stall current is measured at the point when the motor has torque that the RPM goes down to zero. This is also the point at which the most waste heat will be dissipated into the motor body.
{% endtab %}

{% tab title="Free Speed" %}
**Free Speed** is the **angular velocity** that a motor will spin at when powered at the **Operating Voltage** with zero load on the motor’s output shaft. This RPM is the fastest **angular velocity** the motor will ever spin at. Once the motor is under load its **angular velocity** will decrease.

{% hint style="info" %}
_Learn more about angular velocity in the_ [_Core Concepts_](broken-reference) _section_
{% endhint %}
{% endtab %}

{% tab title="Operating Voltage" %}
**Operating Voltage** is the expected voltage that the motor will experience during operation. If a robot is built using a 12 volt battery the **Operating Voltage** of the motor will be 12 volts. When controlling the RPM of the motor the DC speed controller will modulate the effective voltage seen by the motor. The lower the voltage seen by the motor the slower it will spin. DC motors have a maximum rated voltage if this voltage is exceeded the motor will fail prematurely.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
The key metrics defined above are interrelated. Take some time to familiarize yourself with the definitions and how they connect together.
{% endhint %}

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M8MarlMx5meMXBAcMX_%2F-M8MjbITl7U1Z3GF12lg%2Fimage.png?alt=media&#x26;token=23cc8cf8-3552-45fe-96fe-a2fd6d91e5cc" alt=""><figcaption></figcaption></figure>

The prototypical performance graph of a Brushed DC motor can be used to estimate the performance of a motor. In most cases amperage, the unit of measurement for current, is the easiest value to find as it can be reported by the REV Control Hub ([REV-31-1595](https://www.revrobotics.com/rev-31-1595/)) and Expansion Hub ([REV-31-1153](https://www.revrobotics.com/rev-31-1153/)).

### Preventing Premature Motor Failure&#x20;

In order to ensure that an electric motor lasts as long as possible a few rules of thumb should be kept in mind:

* **Smooth loading** - large torque spikes or sudden changes in direction can cause the wear and premature failure of gear box components. This is only an issue when the torque spike exceeds the rated stall torque of the motor. When shock loading is necessary, it is best to utilize mechanical braking or a hard stop that absorbs the impact instead of the motor.
* **Overheating** - when a motor is loaded at near its maximum operating torque it will produce more waste heat than when operating at a lower operating torque. If this heat this allowed to build up the motor can wear out prematurely or fail spontaneously.

{% hint style="info" %}
The Core Hex motor can run for approximately 4 hours continuously before overheating at near maximum torque loading.
{% endhint %}

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MkxSTCiBXSImLUpgg3a%2F-MkxTx7rWGPS61t1vhRb%2Fwaste%20power%20chart%20-%20motor%20guide%20preventing%20premature%20motor%20failure.png?alt=media&#x26;token=8ffd06bb-070e-4bce-b30a-46f7074f0663" alt=""><figcaption></figcaption></figure>

* **Poorly supported output shaft**, most motor output shafts are not designed to take large thrust forces or forces normal to the shaft. Bearings need to be used to support the axle when loads in these directions are expected.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8MarlMx5meMXBAcMX_%2F-M8MhYlSbdgM5CBTcLsw%2F7.png?generation=1590609462320338&#x26;alt=media" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
_To learn more about how to properly support motion visit the_ [_supporting motion_](broken-reference) _page_
{% endhint %}

## REV Motor Specifications

REV DUO Robotics motors come in two types, [HD Hex Motors](broken-reference) and [Core Hex Motors](broken-reference). All REV DUO Motors have a Hex Shaft or female hex coupler as the output from its gearbox. The Hex Shaft is extremely reliable at transmitting torque without being reliant on set screws that can come loose or not be tightened sufficiently. REV DUO motors also include keyed locking connectors for both the motor power and the built-in encoder.&#x20;

{% hint style="info" %}
_For more information on the encoder see the Control System Guide_
{% endhint %}

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M8MarlMx5meMXBAcMX_%2F-M8N2tQzyjYft6IXAWR3%2FScreenshot%20(4).png?alt=media&#x26;token=bed0b70d-86d8-4ffa-8a99-d94f8f7053ef" alt=""><figcaption></figcaption></figure>

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8MarlMx5meMXBAcMX_%2F-M8MhYlWc2lieDE0X1Fg%2F11.png?generation=1590609462333072&#x26;alt=media" alt=""><figcaption></figcaption></figure>
