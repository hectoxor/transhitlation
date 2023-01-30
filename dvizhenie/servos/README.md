---
description: Servo Basics
---

# Servos

Servo motors are a specialized kind of motor which can be controlled to move to a specific angle instead of continuously rotating like a DC motor. Instead of a hex output shaft like the DC motor, servos have an output spline. A **spline** is a specific groove pattern cut into the shaft which allows the rotation of the servo motor to be transmitted to the attached Aluminum Servo Horn ([REV-41-1363](https://www.revrobotics.com/rev-41-1363/)) or [Servo Adapter](https://www.revrobotics.com/ftc/motion/wheels-hubs-adapters/). Splines are like keys, so only matched types will fit together. The REV Robotics Servos all use a 25T spline pattern. If the gears or spline of the REV Robotics Smart Robot Servo ([REV-41-1097](https://www.revrobotics.com/rev-41-1097/)) become damaged, they are replaceable using a Replacement Gear Set ([REV-41-1168](https://www.revrobotics.com/rev-41-1168/)).&#x20;

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FH9K1InCLC1ZxIkdPJt31%2Fuploads%2FQQWfPA2jvlDUhJOiFNuW%2FREV-41-1097%20SRS%20drawing.png?alt=media&#x26;token=f0e899ab-11df-4aa2-bb64-7eb02273adef" alt=""><figcaption></figcaption></figure>

Common servo motors take a programmed input signal range and map that to an angular range. For example, for a servo with a 270° range, if the input range was from 0 to 1 then a signal input of 0 would cause the servo to turn to point -135°. For a signal input of 1, the servo would turn to +135°. Inputs between the minimum and maximum have corresponding angles evenly distributed between the minimum and maximum servo angle.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MB_vrFI_mJbhAOGXIO5%2F-MB_yzhf7dnGkYfx6zkp%2FServo_270_Range_Full_Green-01.png?alt=media&#x26;token=db791fac-0f86-42d8-9651-1c0e42ae87ad" alt=""><figcaption></figcaption></figure>

## Servo Adapters

REV Robotics Servo Adapters fit 25T spline servos like the REV Robotics Smart Robot Servo. In addition to the variety pack of generic servo horns which come with the Smart Robot Servo, there are four other custom servo adapters which make using servos with the REV 15mm Building System easy.

**Servo Gear Adapters** convert a 25T servo into 15 tooth Delrin gear which is compatible with the other REV Robotics Plastic Gears.&#x20;

**Servo Shaft Adapters** convert a 25T spline servo output shaft into a female 5mm hex socket.  This adapter can be used to drive a hex shaft directly.

**Aluminum Servo Horns** have a tapped hole pattern that can be directly mounted to any of the REV Robotics gears, wheels, or sprockets with the Motion Pattern.

**Aluminum Double Servo Arms** ([REV-41-1820](https://www.revrobotics.com/rev-41-1820/)) **** have two tapped holes that can be directly mounted to any of the REV Robotics extrusion, channel, or brackets.&#x20;

## Servos with the Control Hub and Expansion Hub

Teams should be aware of the number of servo motors they attach to each Hub. The Control Hub ([REV-31-1595](https://www.revrobotics.com/rev-31-1595/)) and Expansion Hub ([REV-31-1153](https://www.revrobotics.com/rev-31-1153/)) only can handle 5 Amps through all 6 servo ports. The maximum current a servo will draw is 2.0 Amps, called the stall current. A servo will draw the stall current when it is applying the maximum force, but it is not moving. For example, a servo can stall when a mechanism needs to hold something or a heavy object blocked the path of the servo motion.&#x20;

Normally servos do not draw the maximum current, but teams do not know what might happen during matches. To protect against overdrawing the current on the Hub, only attach 2 servos to a Control Hub or Expansion Hub. Teams can safely use 4 servos: 2 servos on the Control Hub and 2 servos on the Expansion Hub.

If more power is required, consider using the REV Servo Power Module ([REV-11-1144](https://www.revrobotics.com/rev-11-1144/)). It is a 6V 90W power injector that enables the use of high-power RC servos in applications where a robot controller cannot provide adequate power.
