# Gears

## Gear Basics&#x20;

Gears have teeth that mesh with other gears in order to transmit torque. Gears can be used to change the speed, torque (turning force), or direction of a motor’s original output. For gears to be compatible with each other, the meshing teeth must have the same shape (size and pitch).

{% hint style="info" %}
Gears offer more flexibility in transforming motion than sprockets and chain because there are a larger variety of gear sizes available.
{% endhint %}

There are many different types of gears; one of the simplest and most commonly used is a **spur gear**, and that is the gear type used in the REV DUO Build System. **Spur gears** consist of a disk with straight teeth projecting radially (outward from the center) and these gears will only mesh correctly with other gears if they are on parallel shafts.

### Anatomy of a Spur Gear

Common and important features of a spur gear are highlighted in the image below.&#x20;

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M9UyJQ58gxmBWnvU4aJ%2F-M9UzF3Da37nO8IlnZIM%2F1.png?generation=1591822059637529&#x26;alt=media" alt=""><figcaption></figcaption></figure>

{% tabs %}
{% tab title="Number of Teeth" %}
_**Number of Teeth (N)**_ is the total count of the number of teeth (projections) around the whole circumference of a gear. For gears with very few or very large teeth it is easy to simply count the number of teeth. However, for gears with a higher number of teeth, or when the teeth are smaller, attempting to count the teeth is not very practical or accurate.&#x20;
{% endtab %}

{% tab title="Module" %}
_**Module (M)**_ represents the amount of **pitch diameter** in mm per tooth. Gears with a higher **module** will have bigger teeth. **Module (M)** can be calculated using some combination of pitch diameter (PD), number of teeth(N), or outside diameter(OD).&#x20;

Equations for calculating module:&#x20;

* $$M = PD/ N$$&#x20;
* $$M = OD/(  N + 2)$$&#x20;

**To help with calculations:** REV Plastic Gears have a 0.75 module, while REV Metal Gears have a 0.8 module.
{% endtab %}

{% tab title="Pitch Diameter " %}
_**Pitch Diameter (PD)**_ is the imaginary circle that mates with any other gear’s pitch diameter when the gears are properly spaced. The pitch diameter will always be smaller than the outside diameter of a gear.

When creating simplified models for gears, first create a circle with the **pitch diameter** for each gear used in the system then constrain the circles tangent (just barely touching) to each other. **Pitch Diameter (PD)** can be calculated using some combination of module(M), number of teeth (N), or outside diameter (OD).

![](broken-reference)

Equations for calculating pitch diameter:&#x20;

* $$PD = M ×N$$&#x20;
* $$PD = (OD × N) / (N + 2)$$&#x20;
* $$PD = OD -2M$$&#x20;
{% endtab %}

{% tab title="Outside Diameter " %}
_**Outside Diameter**_ _**(OD)**_ is the true outside diameter of a gear. The **outside diameter** will always be larger than the **pitch diameter**. The **outside diameter** should be used when checking for interference when placing gears very close to other structures. **Outside Diameter (OD)** can be calculated using the formula below.

Equations for outside diameter:&#x20;

* $$OD = ( N+2) × M$$&#x20;
{% endtab %}
{% endtabs %}

### Product Specifications&#x20;

The REV DUO Build System includes both [Metal](https://www.revrobotics.com/competition/ftc/motion/rotary-motion/gears/metal-0-8-mod-gears/) and [Plastic ](https://www.revrobotics.com/competition/ftc/motion/rotary-motion/gears/metal-0-8-mod-gears/)Gears. The table below covers some of the basic specifications for the different types of gears.&#x20;

|                    | Plastic             | Metal             |
| ------------------ | ------------------- | ----------------- |
| **Module**         | 0.75                | 0.8               |
| **Pressure Angle** | 20°                 | 20°               |
| **Material**       | Acetal (Delrin/POM) | 7075-T6 Aluminum† |
| **Thickness**      | 15mm                | 5mm               |

{% hint style="info" %}
_† The majority of Metal Gears in the REV DUO Build System are made using aluminum. There are three exceptions. The 12 Tooth and 28 Tooth Gears are made out of Sintered Steel. The 12 Tooth Pinion Gear is made out of Machined Brass._
{% endhint %}

Both the Metal and Plastic Gears are compatible with [M3 hardware](https://www.revrobotics.com/ftc/hardware/fasteners/) with a 8mm pitch.&#x20;

#### Plastic Gears&#x20;

All REV DUO Plastic Gears have a M3 bolt hole mounting pattern that is on an 8mm pitch. This makes it easy to directly mount REV Robotics [Brackets](https://www.revrobotics.com/ftc/structure/) and [Extrusion](https://www.revrobotics.com/ftc/structure/15mm-extrusion/) to gears. The webbed design, combined with a wide face width and small tooth profile, increases the gear strength without adding significant weight. REV Robotics Plastic Gears are designed to fit a 5mm hex shaft which eliminates the need for special hubs and setscrews.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M9UyJQ58gxmBWnvU4aJ%2F-M9UzF3Pahn4-ljhLxFF%2F13.png?generation=1591822059712508&#x26;alt=media" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
**REV Metal Gears are NOT compatible with REV Plastic Gears.** Gears from other building systems may have a very similar tooth profile but are not an exact match. It may be possible to use the two gears systems together successfully in some situations, but it is not recommended.
{% endhint %}

#### Metal Gears

Metal Gears are designed to work with [REV 5mm Hex Shafts](https://www.revrobotics.com/ftc/motion/bearings-linear-slides-pillow-blocks/) in high-load applications. REV DUO Metal Gears also have a M3 hole pattern, but this pattern focuses on allowing gears to be doubled up for additional strength. In general, the REV DUO Metal Gears have a higher yield strength than the REV DUO Plastic Gears, especially when the metal gears are doubled up. Thickness of the gear teeth, known as face width, is a core component of gear strength.&#x20;

{% hint style="info" %}
The face of the REV DUO Metal Gears displays the gears tooth count to help with calculations!
{% endhint %}

All REV DUO Metal Gears are narrower than plastic gears, allowing for compact drivetrains and gearboxes within the same 15mm width as the Extrusion and Punch Tube ([REV-41-1453](https://www.revrobotics.com/rev-41-1453/)).&#x20;

## Using Gears as a Powertrain&#x20;

Meshing two or more gears together is known as a **gear train**. Selecting the gears in the gear train as larger or smaller relative to the input gear can either increase the output **speed**, or increase the output **torque** but the **total power** is not affected.

{% hint style="info" %}
_Physics concepts, like speed and power, have a lot of applications in the REV 15mm Build System. Click here to learn more about them._&#x20;
{% endhint %}

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M9Zg_T1krecrlLn0n8a%2F-M9ZlOwZcPzzbfio3rVx%2Fimage.png?alt=media&#x26;token=c94ad051-24c9-4544-a71a-7dafd53c369b" alt=""><figcaption></figcaption></figure>

A **gear ratio** is the ratio of the sizes of two gears. For instance, in the image below, the **input gear** is a 15 tooth gear and the output gear is a 72 tooth gear. So, the **gear ratio** is 72T:15T. The **ratio** in size from the input (driving) gear to the output (driven) gear determines if the output is faster (less torque) or has more torque (slower). The gear ratio is proportional to the speed and torque changes between them.

{% hint style="info" %}
_To learn more about gear ratios and how they affect speed and torque check out the_[ _Gear Ratio_ ](broken-reference)_section_&#x20;
{% endhint %}

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M9Zm_nDCSZRRbIsBVPX%2F-M9Zv0I3Rjynk31Eeerb%2Fimage.png?alt=media&#x26;token=c16473b1-849c-4132-89e7-3cc389c786fa" alt=""><figcaption></figcaption></figure>

In the image above, the 15 tooth input gear is rotating clockwise. As the input gear rotates, it pushes down on the output gear where the teeth are meshed. This action transmits the motion to the output gear, but forces the output gear to rotate in the opposite direction of the input gear.&#x20;

{% hint style="info" %}
_One way to change change the direction of rotation in a gear train is to add **idlers**. **Idlers** sit between the input and output gear in a gear train and can help you manipulate the rotation of the output gear. To learn more about idlers check out the_[ _Idler_](broken-reference) _section_&#x20;
{% endhint %}

{% hint style="warning" %}
If you are using gears to transmit motion over long distances, like in a drivetrain, please check out the[ Gear Train](broken-reference) section to understand more about how to properly employ that sort of mechanism.&#x20;
{% endhint %}

## How to Use REV  DUO Gears?

As mentioned in the [Specifications ](broken-reference)section, DUO Gears work with the 5mm Hex Shaft to drive motion along a a gear train. To learn more about using Hex Shafts and proper motion support and constraint visit the pages linked below:

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

### Gear Spacing&#x20;

In order for gears to work effectively, and not become damaged, it’s important that the **center-to-center distance** is correctly adjusted. The gears in DETAIL A, of the figure below, may work under very light load, but they will certainly not work and will skip under any significant loading. The gears in that example are too far apart and so the teeth of each gear barely contact each other. The gears in DETAIL B are correctly spaced and will provide smooth and reliable operation.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-M9_EIVj36TXLkG6buP6%2F-M9_LMrZk5oLsWbT9-CE%2Fimage.png?alt=media&#x26;token=674b5835-8166-4d64-8434-20404acfd72d" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
_To learn more about calculating center-to-center distance for Gears visit the_ [_Spacing and Center to Center Distance_](broken-reference) _section_&#x20;
{% endhint %}

### Gear Alignment Mark

Sometimes in a design it may be desirable to stack together multiples of the same gear on a shaft to increase the load carrying capacity of the gears. In the case where the number of teeth on the gear is not divisible by six, because of how they are oriented when put onto the hex shaft, the teeth may not be aligned between the two gears. To ensure all of the gears are clocked the same way, use the alignment shaft notch to put all the gears on the shaft with the same orientation.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M9UyJQ58gxmBWnvU4aJ%2F-M9UzF3R6QGRqB1YMa7z%2F15.png?generation=1591822059652653&#x26;alt=media" alt=""><figcaption></figcaption></figure>

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M9UyJQ58gxmBWnvU4aJ%2F-M9UzF3QFi2GCh80_247%2F14.png?generation=1591822059617958&#x26;alt=media" alt=""><figcaption></figcaption></figure>

Being aware of the alignment mark will ensure all of the gear teeth are aligned on the shaft. The figure below is an example of a basic robot arm which may have to lift a heavy load. Using two gears to lift the arm doubles the material interfacing with the hex shaft and will allow the arm to perform with heavier loads.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F15mm%2F-M9UyJQ58gxmBWnvU4aJ%2F-M9UzF3SjHNz3sVEuRD3%2F16.png?generation=1591822059682956&#x26;alt=media" alt=""><figcaption></figcaption></figure>
