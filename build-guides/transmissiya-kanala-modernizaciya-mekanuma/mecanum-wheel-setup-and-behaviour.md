# Mecanum Wheel Setup and Behaviour

Mecanum wheels, when properly set up on a drivetrain, allow for omni-directional movement. Each Mecanum Wheel Set ([REV-45-1655](https://www.revrobotics.com/rev-45-1655/)) comes with a two right (REV-41-1656) and two left (REV-41-1657) mecanum wheels. This is determined by the direction of the leading edge of the rollers. If the rollers point left it is a left wheel and if they point right it is a right wheel.&#x20;

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MEdFLXTiGafr6U3r\_25%2F-MEdOvGHyh9ZFSpewGH\_%2Fview%204.svg?alt=media\&token=af5e84d5-96f5-458a-b8f5-b73c7075eb97)

Each side of the chassis needs one left and one right wheel. Mecanum Chassis also require four motors for operation.‌

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGEhbw8k2D2JwY4u7qV%2FMVD\_Top%20-%20Arrows\_GB.svg?alt=media\&token=f4ef8a55-e246-4df0-8c6b-279ea88b5fa5)

To know if your Mecanum Wheels are properly configured look from the top down on the drivetrain. Following diagonal lines created from the angle of the rollers should form an "X" as shown above.‌

### Mecanum Wheel Drivetrain Behavior

Running all four wheels in the same direction at the same speed will result in a forward/backward movement, as the longitudinal force vectors add up but the transverse vectors cancel each other out, as shown below.‌

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGElkhKXVl-5E9PyleO%2FMVD\_Forward\_Reverse\_GB%20REDo.svg?alt=media\&token=40fe8463-8f23-4136-a639-99bf049a1577)

When both wheels on one side of the drivetrain are moving in one direction while the other side is moving in the opposite direction results in stationary rotation of the drivetrain. The transverse vectors cancel out but the longitudinal vectors combine to generate rotation around the central vertical axis of the drivetrain, as shown below.‌

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGElp8x9TzAzBG5F\_NH%2FMVD\_Spin\_GB%20Redo.svg?alt=media\&token=6877456d-f1c9-4ec9-af3d-e1582c81abe2)

When the right mecanum wheels run in one direction while the left mecanum wheels run in the opposite direction allows for a strafing movement, as the transverse vectors add up but the longitudinal vectors cancel out.‌

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGEo9JBskv1dec5kwjH%2FMVD\_Strafe\_GB%20Redo.svg?alt=media\&token=f5bd20a9-662a-4489-9791-6c3227f2ab63)

Using the above concepts in tandem through varying motor power to each wheel type allows for the drivetrain to move in different, angled vectors.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGEuHO5rL_qf6RIPAes%2F-MGEy5xLE0nUJxvnvdtc%2FMVD_Vector_GB%20redo.svg?alt=media&#x26;token=d793e5b0-2c99-4929-b220-7781c66d54c2" alt=""><figcaption></figcaption></figure>
