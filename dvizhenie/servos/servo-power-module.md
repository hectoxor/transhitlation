# Servo Power Module

## Servo Power Module Basics

The REV Servo Power Module ([REV-11-1144](https://www.revrobotics.com/rev-11-1144/)) is a 6V 90W power injector that enables the use of high-power RC servos in applications where a robot controller cannot provide adequate power.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8VuTXTeaMyPtvVrNSd%2F-M8WMcrnMWEB7n-inTqu%2F2.png?generation=1590771487323342&#x26;alt=media" alt=""><figcaption></figcaption></figure>

### Product Specifications

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FH9K1InCLC1ZxIkdPJt31%2Fuploads%2FyiWxbuAKk1gmi9N16RaR%2Fspm%20labeled.png?alt=media&#x26;token=b436763e-86a1-430a-a811-970f6114c5c6" alt=""><figcaption></figcaption></figure>

| Key Terms                                                                                      | Key Metrics          |
| ---------------------------------------------------------------------------------------------- | -------------------- |
| **Nominal Input Voltage**                                                                      | 12V                  |
| **Operating Voltage Range**                                                                    | 7.0V - 20V           |
| **Minimum Startup Voltage**                                                                    | 9.0V                 |
| **Output Voltage**                                                                             | 6V                   |
| **Number of Channels**                                                                         | 6                    |
| <p><strong>Max. Total Output Current</strong></p><p><strong>(across all Channels)</strong></p> | 15A                  |
| **Max. Total Output Power**                                                                    | 90W                  |
| **Size**                                                                                       | 3.6” x 1.52” x 0.81” |
| **Weight**                                                                                     | 2.0oz/57g            |

## How to Use&#x20;

### Electrical Connections

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8VuTXTeaMyPtvVrNSd%2F-M8WMcrpi_Pd87PP76iS%2F4.png?generation=1590771487272705&#x26;alt=media" alt=""><figcaption></figcaption></figure>

The Servo Power Module has two screw terminals for 12V power input. It is recommended to use ring or fork terminals designed for #6 or M3 screw terminals.

Using an appropriate wire gauge, 18 AWG or larger, tightly crimp either a ring or fork terminal on the wire. Insert the crimped terminal into the screw terminal and tighten the screw.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M8VuTXTeaMyPtvVrNSd%2F-M8WMcrqMsXUzLIElogM%2F5.png?generation=1590771487662184&#x26;alt=media" alt=""><figcaption></figcaption></figure>

The input and output channels accept standard 3-wire 0.1” pitch servo/PWM cables. Please refer to the figure above or the case markings for proper orientation.

### Status LEDs

Each channel has a corresponding status LED that will indicate the sensed state of the connected PWM signal. The table below describes each state’s corresponding LED pattern.

| **State**             | **Pattern**    |
| --------------------- | -------------- |
| No Signal             | Blinking Amber |
| Left/Reverse Signal   | Solid Red      |
| Center/Neutral Signal | Solid Amber    |
| Right/Forward Signal  | Solid Green    |

### Over-Current Shutdowns&#x20;

If the Servo Power Module detects a total output current larger than 15A it will enter a shutdown mode where the 6V output is disabled until the over-current condition has remedied. While in shutdown the blue power LED will turn off, dim, or flicker indicating the over-current condition is still present.

In the case of frequent over-current shutdowns, ensure that the total stall current of all connected servos does not exceed 15A.
