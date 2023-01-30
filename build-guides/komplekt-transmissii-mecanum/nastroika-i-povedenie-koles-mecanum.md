# Настройка и поведение колес Mecanum

Колеса Mecanum, при правильной установке на трансмиссию, обеспечивают всенаправленное движение. Каждый комплект колес Mecanum (REV-45-1655) поставляется с двумя правыми (REV-41-1656) и двумя левыми (REV-41-1657) колесами Mecanum. Это определяется направлением передней кромки роликов. Если ролики направлены влево, то это левое колесо, а если вправо - правое.

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MEdFLXTiGafr6U3r\_25%2F-MEdOvGHyh9ZFSpewGH\_%2Fview%204.svg?alt=media\&token=af5e84d5-96f5-458a-b8f5-b73c7075eb97)

Для каждой стороны шасси необходимо одно левое и одно правое колесо. Для работы шасси Mecanum также требуется четыре двигателя.

![Вид сверху](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGEhbw8k2D2JwY4u7qV%2FMVD\_Top%20-%20Arrows\_GB.svg?alt=media\&token=f4ef8a55-e246-4df0-8c6b-279ea88b5fa5)

Чтобы узнать, правильно ли настроены колеса Mecanum, посмотрите сверху вниз на трансмиссию. Диагональные линии, образованные углом наклона роликов, должны образовывать букву "X", как показано выше.

**Поведение колесной трансмиссии Mecanum**

Движение всех четырех колес в одном направлении с одинаковой скоростью приведет к движению вперед/назад, поскольку векторы продольной силы складываются, а векторы поперечной силы отменяют друг друга, как показано ниже..‌

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGElkhKXVl-5E9PyleO%2FMVD\_Forward\_Reverse\_GB%20REDo.svg?alt=media\&token=40fe8463-8f23-4136-a639-99bf049a1577)

Когда оба колеса с одной стороны трансмиссии движутся в одном направлении, а другая сторона движется в противоположном направлении, это приводит к стационарному вращению трансмиссии. Поперечные векторы аннулируются, но продольные векторы объединяются, создавая вращение вокруг центральной вертикальной оси трансмиссии, как показано ниже.

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGElp8x9TzAzBG5F\_NH%2FMVD\_Spin\_GB%20Redo.svg?alt=media\&token=6877456d-f1c9-4ec9-af3d-e1582c81abe2)

Когда правые колеса Mecanum движутся в одном направлении, а левые колеса Mecanum движутся в противоположном направлении, это позволяет выполнять движение с перекладкой, так как поперечные векторы складываются, а продольные векторы аннулируются.

![](https://2589213514-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGAlk3hA20qNrkaOKFl%2F-MGEo9JBskv1dec5kwjH%2FMVD\_Strafe\_GB%20Redo.svg?alt=media\&token=f5bd20a9-662a-4489-9791-6c3227f2ab63)

Использование вышеупомянутых концепций в тандеме посредством изменения мощности двигателя для каждого типа колес позволяет трансмиссии двигаться в различных угловых векторах.

<figure><img src="https://2589213514-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M5yw0n8IneF5-9ybLjT%2F-MGEuHO5rL_qf6RIPAes%2F-MGEy5xLE0nUJxvnvdtc%2FMVD_Vector_GB%20redo.svg?alt=media&#x26;token=d793e5b0-2c99-4929-b220-7781c66d54c2" alt=""><figcaption></figcaption></figure>
