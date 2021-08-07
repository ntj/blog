---
title: "Fehlvorstellungen"
date: 2021-07-25
draft: false
categories: ["Thoughts"]
---

In der Forschung zu Didaktik der Informatik spielen Fehlvorstellungen und ihre Behebung eine große Rolle.
Fehlvorstellungen sind falsch internalisierte Vorstellungen, wie etwas funktioniert. Sie erschweren die Aneignung und das Verstehen eines Lerngegenstandes.

Die meisten Menschen kommen mit Computer, dem Internet und Informationstechnologie im Allgemeinen früher oder später in Berührung, der Schulunterricht vermittelt aber nur unzureichend die notwendigen Grundlagen, sei es, weil kein flächendeckender Informatikunterricht existiert oder sich die Technik schnell ändert oder weil er zu spät beginnt.

Es ist interessant, darüber nachzudenken und zu überlegen, ob einem diese Fehlvorstellungen schon einmal begegnet sind.

Ich erinnere mich an eine Situation, als ich mit jemanden sprach und es ging über die Rechtevergabe in einem Unix-System. Also chmod 755 und solche Sachen. Wir haben also darüber gesprochen, ob es nun 755 oder 775 sein sollte und ich glaube, mich zu erinnern, mein Gegenüber hätte in einer Tabelle nachschlagen wollen, was diese Nummern konkret bedeuten. Also es war ihm in dem Moment nicht bewusst, dass es sich um die Dezimalrepräsentation von Binärzahlen handelt und man an den entsprechenden Binärzahlen, also 111 101 101 dann die Rechte für rwx für User, Group und All ablesen kann.

Aber worin genau liegt da die eigentliche Fehlvorstellung? Er wusste also nicht, wenn wir über Zahl, die wie eine Dezimalzahl aussieht, sprechen, dass wir nicht die Dezimalzahl meinen, sondern die einzelnen Ziffern die Dezimalrepräsentation der entsprechenden Binärzahlen sind.

Ich glaube, solchen Fehlvorstellungen kann man nur mit einem sehr guten Informatikunterricht begegnen. Und der Bezug zur Rechtevergabe in einem Unix-System müsste dann bei der Behandlung der Binärzahlen gezogen werden. Dann ist es logisch, dann ist es verständlich und dann vergisst man es auch nicht mehr so schnell und kann es sich herleiten.

_This is day 51 of my [#100daystooffload](https://100daystooffload.com/) series, a challenge to write 100 blog posts in a year._