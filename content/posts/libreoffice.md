+++
title = "Code beisteuern zu Open Source Projekten"
date = 2021-02-05T20:06:45+01:00
images = []
tags = []
categories = []
draft = false 
+++
Schon seit geraumer Zeit versuche ich, nicht nur Quellcode zu schreiben oder meine Repositories als freie Software verfügbar zu machen, sondern auch Quellcode zu großen,
existierenden Repositories hinzuzufügen. "Contribute to Open-Source-Projekten" ist meiner Ansicht nach hauptsächlich so gemeint und für mich die Kür des Programmiererinnendaseins.

## Django

Richtig aktiv wurde ich zum ersten Mal, nachdem ich den Talk "[Your Webframework Needs You](https://www.youtube.com/watch?v=LjTRSH0pNBo&list=PL2NFhrDSOxgXXUMIGOs8lNe2B-f4pXOX-&index=28)" von Carlton Gibson auf der
DjangoCon2019 gesehen hatte. Sein Elan hat mich begeistert und mir wurde klar, wie wichtig es
ist, selbst Quellcode beizusteuern, wenn man ein Open-Source-Projekt gerne weiternutzen möchte.

Nach der Konferenz fand ein [Sprint](https://en.wikipedia.org/wiki/Hackathon#Code_sprints) statt, auf dem ich sofort loslegen konnte.
Es gab Beginner's Tickets, von denen ich eins auswählte und ich habe an dem Tag auch einen
kleinen Pull-Request veröffentlicht.

Aber leider ging es nicht darüber hinaus. Es gab aus meiner Sicht zu wenige Aufgaben, an
denen man sich erst einmal ausprobieren konnte, um die Codebasis kennenzulernen.

Trotzdem hatte ich im Anschluss die Django-User-Mailingliste für mich entdeckt und die ein oder andere Frage dort beantwortet. Und auch heute noch, obwohl ich kaum mehr eine Zeile
Django schreibe, logge ich mich immer mal bei Discord ein und wenn ich eine klassische Frage zum ORM, zu Jinja2 oder Models, Views und Forms sehe, beantworte ich sie gerne.

Fazit: Auch wenn ich kein Django Developer im eigentlichen Sinne geworden bin, weil ich
keinen Quellcode zu Django beigesteuert habe, hatte der Aufruf auf der DjangoCon einen
großen Effekt auf mich und ich glaube, ich konnte und kann der Django Community aushelfen,
in dem ich in ihren Kanälen dazu beitrage, Einsteiger und Mainstreamfragen nicht unbeantwortet zu lassen.

## LibreOffice

Im Januar 2021 bin ich auf die Developer-Seiten von LibreOffice aufmerksam geworden und ich wollte versuchen, ob ich hier vielleicht an einem großen Projekt mitschrauben kann.
Und das hat geklappt! Ungefähr eine Woche verging beginnend vom ersten Clonen des Repos bis zum erfolgreichen Durchlauf meines Patches auf der CI-Plattform Jenkins.

Hier möchte ich einmal auflisten, was dabei gut lief und wo es zunächst klemmte:
* Die Dokumentation aller ersten Schritte ist super, der Build auf meinem ArchLinux-System klappte auch ohne Probleme
* Die Liste der EasyHacks ist übersichtlich und ich habe auch gleich ein wirklich ganz leichtes Ticket gefunden.

Hier hat es geklemmt:
* Mein Jenkins-Build war nicht erfolgreich. Der Log war zwar aussagekräftig, aber da das Neubauen des Quellcodes so lange braucht, war es schwierig für mich zu entscheiden,
wie ich vorgehen sollte. Neu bauen mit Debugsymbolen, nur die Testsuite bauen, die fehlschlug? Auch tauchte der Fehler nur bei einem Build mit dem Compiler clang auf, nicht mit gcc. Sollte ich versuchen, meine Entwicklungsumgebung auch mit clang zu kompilieren? Hier wäre noch eine Seite hilfreich gewesen, "Troubleshoot failing Jenkins builds". Vielleicht wäre auch eine Seite "Best-practices" von erfahrenen Kontributoren nützlich, auf der sie ihr Setup und ihre Konfiguration des make-Befehls teilen, also all das, was über die pure Dokumentation der Optionen hinausgeht.

Das war wieder top:

* Im IRC-Channel wurde mir geholfen, auf meine Fragen habe ich eine Antwort
bekommen und es ist einfach super, wenn man nicht weiß, was los ist, eine seiner
vielen Fragen irgendwo hinpacken kann und auch eine Antwort erhält.

Letztendlich hat eine Aktualisierung meines lokalen Branches auf den aktuellen remote-master dazu geführt, dass der Build dann erfolgreich durchlief. Also lag es nicht an meinem Patch! Ich war genau zu dem Zeitpunkt fertig, an dem ich spätestens fertig sein wollte, Sonntag Abend in derselben Woche.

Fazit: LibreOffice ist ein sehr umfangreiches Projekt, trotzdem ist es sehr gut aufgestellt, neuen Kontributoren den Einstieg zu erleichtern. Ich glaube, es lohnt sich wirklich, die Liste der EasyHacks gut zu pflegen. Aber wenn man wirklich neue Entwickler/innen ins Boot holen möchte, denke ich, spielen noch weitere Dinge eine Rolle:
1. Keine Newbie-Frage unbeantwortet lassen.
2. Neue Kontributoren, wenn es geht, da einbinden, wo es darum geht, immer wiederkehrende
Fragen zu beantworten. Auch wenn man eine super simple Frage stellt, ist es schön, nicht nur mit einer Zwei-Silben-Antwort und einem Link abgespeist zu werden.
3. Nicht nur einen Link zu einer Dokumentation schicken, lieber noch einen erklärenden Satz dazu schreiben. Wenn man eine Funktion gut kennt, ist deren Dokumentation meist verständlich, wenn man sie nicht kennt, manchmal nicht.

Und am allerwichtigsten:
**Aufrufe zur Mithilfe haben einen großen Effekt.**
