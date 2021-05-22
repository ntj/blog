---
title: "Freie Software weiterdenken"
date: 2021-05-22
draft: false
categories: ["FOSS"]
---

Zur Zeit findet eine spannende Debatte auf der deutschsprachigen Mailingliste der FSFE statt. Es ging zunächst um nicht-kommerzielle Lizenzen und die Commons Clause.

Software, die unter einer Commons Clause steht, (wie z. B. [WorkAdventure](https://workadventu.re/faq#license)) wird nicht als freie Software angesehen, weil sie gegen die erste der [vier FOSS-Freiheiten](https://fsfe.org/freesoftware/) verstößt, denn Nutzer:innen können die Software nicht mehr zu allen Zwecken verwenden. Dieser Punkt ruft oft Unverständnis hervor. Aus Sicht der Entwickler:innen ist es sicher nachvollziehbar, dass man ausschließen möchte, dass sich jemand ohne eigenes Zutun an einem Produkt bereichert, in welches man selbst viel Arbeit und Zeit investiert hat.

Daraus entspannte sich Diskussion darüber, ob und inwiefern die vier Freiheiten für aktuelle Fragestellungen keine passenden Antworten mehr liefern.

Zum Beispiel kann eine Software frei sein (und wer ist nicht Freund:in freier Software) und trotzdem zu unethischen Zwecken eingesetzt werden. Ein FOSS-Entwickler hat keine Möglichkeit, zu verhindern, dass sein Code in diesen Szenarien verwendet wird.

Matthias Kirschner gibt in einem [Talk](https://media.ccc.de/v/froscon2020-2571-die_kernwerte_der_software_freiheit) eine Überblick über die Historie der vier Freiheiten und argumentiert, dass Software-Lizenzen nicht unbedingt der geeignete Weg sind, um Ziele wie ethisches Handeln in der Welt zu befördern.

Ich habe auf einen [Artikel in der Technology Review](https://www.heise.de/select/tr/2020/5/2007914261339602965) verwiesen, in dem diese Debatte  aufgegriffen wurde und drei zusätzlichhe Forderungen an Software aufgelistet sind, die der Entwickler [Justin Flory](https://jwf.io/) formuliert hat:


- Die Möglichkeit, zu untersuchen, wie eine Software Entscheidungen trifft (etwa ob ein autonomes Auto eher an einen Baum oder in eine Gruppe Schulkinder fahren würde).
- Die Möglichkeit, Verantwortungen zuschreiben zu können (zum Beispiel bei der Anstiftung zum Völkermord in Myanmar durch Facebook-Algorithmen).
- Die Möglichkeit, gegen die Entscheidung einer Software ­Berufung einzulegen.

Aus dem ganzen Thread ergeben sich aus meiner Sicht noch viele Fragen. Um untersuchen zu können, wie eine Software Entscheidungen trifft, benötige ich nicht nur den Quellcode sondern auch Daten. Brauche ich originale Daten oder kann man für jegliche Algorithmen und Programme Mockup-Daten generieren, um diese Untersuchung durchzuführen? Als ich mit Singularity zutun hatte, ging es auch darum, dass Containerisierung sicherstellt, dass die Umgebung, in der der Quellcode läuft, replizierbar ist. Also gleicher Quellcode führt in unterschiedlichen Umgebungen zu unterschiedlichen Ergebnissen. Demzufolge benötige ich also auch diese Informationen, um zu untersuchen, wie die Software Entscheidungen trifft.

Ein anderer Punkt der Debatte war, dass zunehmend Cloudlösungen lokal installierte Anwendungen ablösen und ob nun Open Source Code in der Cloud läuft oder proprietärer Code, aus Sicht der Anwender:innen fühlt sich ein Software-Service unfreier an als ein lokal installiertes Programm. Könnte man hier nicht mit Forderungen zu mehr Dezentralität ansetzen? Ich finds eigentlich spannend zu sehen, wie ein zentrales soziales Netzwerk einen föderierten Clon hat: Twitter und Mastodon. Geht das vom Prinzip auch Webseiten wie Amazon, also ein föderiertes Netz an Händlern, bei denen ich auf alle Produkte zugreifen kann? Dann liegen meine Daten zwar immer noch in der Cloud, aber ich kann den Händler aussuchen, dem ich am Meisten vertraue. Fänd ich schön, wenn man Debatten in dieser Richtung führen könnte.

Und selbst das Argument, dass es sehr schwierig ist, für eine breite Masse konsensfähige Aussagen zu treffen, was als ethisches Verhalten gilt und was nicht, überzeugt mich nicht so richtig.

_This is day 35 of my [#100daystooffload](https://100daystooffload.com/) series, a challenge to write 100 blog posts in a year._