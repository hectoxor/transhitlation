---
description: SRS Programmer Basics
---

# SRS Programmer

The REV Robotics SRS Programmer ([REV-31-1108](https://www.revrobotics.com/rev-31-1108/)) is the key to unlocking all the smart features of the Smart Robot Servo (SRS) ([REV-41-1097](https://www.revrobotics.com/rev-41-1097/)).

Switching between continuous rotation, standard servo, and custom angular modes is easy as pressing a button. The SRS Programmer can not only program the SRS, but it is also acts as a standalone servo tester for any standard RC servo.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8WcLi6koTauMV2xJ63%2F-M8WdOZiJLaHBzbA2oeW%2F1.png?generation=1590776144189561&#x26;alt=media" alt=""><figcaption></figcaption></figure>

### Product Specs&#x20;

The REV Robotics SRS Programmer includes the following features:

* 3 programming modes
  * Continuous rotation
  * Angular limits
  * Reset to factory defaults
* Test modes
  * Automatic sweep
  * Manual position/direction
* Intuitive operation with LED feedback
* Self-powered
* Power-off reminder

| **Mechanical Specifications** |                          |
| ----------------------------- | ------------------------ |
| **Dimensions**                | 70.5mm x 64.5mm x 35.5mm |
| **Weight**                    |                          |

| **Electrical Specifications** |                |
| ----------------------------- | -------------- |
| **Power Source**              | 4 AA batteries |
| **Power Output**              | 6V nominal     |
| **Logic Level (Signal Out)**  | 3.3V           |
| **Output Pulse Width Range**  | 550μs – 2450μs |
| **Center Pulse Width**        | 1500μs         |

† Not Included

## Operating Modes&#x20;

The SRS Programmer has several operating modes for configuring and testing the REV Smart Robot Servo. The following sections describe each operating mode in detail.

{% hint style="warning" %}
Before using the SRS Programmer to switch modes or program your servo motor, check that the batteries are not low. If your SRS Programmer has not been used in a while, please put in a fresh set of batteries to avoid potentially corrupting the firmware of your servo motor.&#x20;
{% endhint %}

### Switching Modes

Follow the steps below to switch a REV Smart Robot Servo between Continuous Mode and Servo Mode. The figure below shows the process to select Continuous Mode.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M8WcLi6koTauMV2xJ63%2F-M8Wf8PNHBydvaPKp5Ax%2FScreenshot%20(25).png?alt=media&#x26;token=74baa009-be7d-4cde-9334-a68fd7beaa35" alt=""><figcaption></figcaption></figure>

1. Connect the SRS to the programmer.
2. Turn on the programmer.
3. Slide the mode switch to the desired mode: C - Continuous, S - Servo.
4. Press and release the PROGRAM button once.
5. The PROGRAM LED should blink and then stay solid indicating success.

### Setting Angular Limits&#x20;

Follow the steps below to set the angular limits for the Servo Mode. The figure below shows an example of setting a left and right limits at -30° and +60° respectively.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlCNxlQ-LJofBQhcpVW%2F-MlCO4tB8H8Yu0ojscjH%2FServo_Full_270_Range_And_Limits-01%20(1).png?alt=media&#x26;token=7a2475d6-978c-4c1e-bfa6-2ecbd2194372" alt=""><figcaption></figcaption></figure>

Start with the SRS already configured in Servo Mode, see section [Switching Modes](broken-reference) for instructions.

1. Connect the SRS to the programmer.
2. Turn on the programmer.
3. Slide the mode switch to S position.
4. This step is optional, but recommended to make it easier to see the valid limit ranges. Please refer to the SRS User's Manual for more information about the valid limit ranges.
   1. Press and release the TEST button twice to enter Manual Test Mode (see [Test Modes](broken-reference) for more information).
   2. Press the PROGRAM button to center the servo at 0°.
   3. Press and release the TEST button once to leave the test mode.
5. Manually rotate the servo to the desired left limit position.
6. Press and release the LEFT button. The LEFT LED will illuminate if the position is valid.
7. Manually rotate the servo to the desired right limit position.
8. Press and release the RIGHT button. The RIGHT LED will illuminate if the position is valid.
9. After both limits are set, press and release the PROGRAM button. The PROGRAM LED should blink and then stay solid indicating success.

### Resetting to Default&#x20;

Follow the steps below to reset the Smart Robot Servo to its default mode and limits. The figure below shows the process to reset to defaults.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MlCNxlQ-LJofBQhcpVW%2F-MlCO9d65k3icfZQy7og%2FServo_270_Range_Full_Green-01.png?alt=media&#x26;token=864f82de-bf70-4fde-acef-28119fa689d8" alt=""><figcaption></figcaption></figure>

1. Connect SRS to the programmer.
2. Turn on the programmer.
3. Slide the mode switch to S position.
4. Press and hold the PROGRAM button for at least 5 seconds.
5. The LEDs will blink and then the PROGRAM LED will stay solid indicating success.

## Test Modes&#x20;

In either Continuous or Servo Modes, pressing and releasing the TEST button cycles through the two test modes:

* 1st press - Automatic Sweep Mode
* 2nd press - Manual Test Mode
* 3rd press - Return to default state

The section below will cover the two different test modes.

{% tabs %}
{% tab title="Automatic Sweep Mode" %}
In Automatic Sweep Mode, the SRS Programmer will automatically sweep the SRS through motions appropriate for its configuration. the table below describes the behavior based on the configured mode.

| **Servo and Programmer Mode** | **Behavior**                 |
| ----------------------------- | ---------------------------- |
| **Continuous Mode (C)**       | Sweeping direction and speed |
| **Servo Mode (S)**            | Sweeping between limits      |
{% endtab %}

{% tab title="Manual Test Mode " %}
In Manual Test Mode the LEFT, PROGRAM, and RIGHT buttons control the movement of the SRS. The table below describes how the SRS will behave based on the configured mode.

![](broken-reference)
{% endtab %}
{% endtabs %}

### Power-off Reminder

If the SRS Programmer is left on for an extended period of inactivity, it will blink every LED as a reminder to shut off power.

## How to Video

{% embed url="https://youtu.be/PJjFdsnw0uY" %}

