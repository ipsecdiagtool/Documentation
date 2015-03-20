###Fünftes Meeting 13:00 - 20.03.2015 (KW12)  
**Teilnehmer:** Andreas Steffen, Tobias Brunner, Jan Balmer, Theo Winter

+ **Aktueller Stand gezeigt:**
	+ Performance Messungen etc. dokumentiert
	+ goProbe Installation dokumentiert
	+ Entscheidung Golang dokumentiert
	+ Erster Prototyp mit Go gezeigt
	
+ **Domain Modell:** Lässt sich mit Golang nicht so gut realisieren weil keine Klassen etc. UML passt nicht ideal. Punkt Domain Modell in Planung in "Modellierung" umgenannt, wir machen jetzt Sequenzdiagramme etc. T.Brunner meint wir sollen aber trotzdem auch Modell mit Packages etc. machen, muss aber nicht so exakt sein. A. Steffen meint Architektur ist nicht so komplex hier, Sequenzdiagramme sind gut.

+ **Experte & Gegenleser:** Ralf Hauser und Josef Joller gem. A.Steffen. Es wird noch ein Meeting für Jan mit J. Joller geben was genau erwartet wird. Wahrsch. auch Freitag 10ter.

+ **Meeting Open Systems AG:** Bisher noch kein Termin abgemacht da viel zu tun. wir werden es übernehmen.

+ **Fragen MTU geklärt:**
	+ Keine automatische Discovery von Gegenüber, wir machen Config file zu Beginn.
	+ Kein auto. verstellen der MTU sondern Log
	+ DEST zwingend, SRC optional
	+ In ESP Paketen hat es JRE
	+ PMTU geht nicht weil ICMP geblockt korrekt, unser Tool ist alternative
	+ Do not fragment verwenden korrekt.
	+ Geplantes Sequenzdiagramm korrekt, aber wir sollen auch Sequenzdiagramm für Sonderfälle modellieren
	+ MTU kann für Route spezifisch gesetzt werden, nicht für Interface, d.h. wir haben nicht eine MTU pro Interface, sondern MTU pro Route.
	
+ **Nächstes Meeting:** Nur mit T.Brunner weil A.Steffen weg ist. Das Meeting darauf wir noch speziell abgemacht weil Ostern ist.

+ **Weiteres Vorgehen:**

	+ **Jan:**
		+ VMs auf Desktop PC Übertragen
		+ VMs fertig dokumentieren
		+ Prototyp Paketverlust anfangen
		+ Prototyp Paketverlust fertig dokumentieren
		+ JNetPcap in Analyse fertig dokumentieren
		
	+ **Theo:**
		+ Risikoanalyse
		+ Überarbeitung NFRs
		+ Prototyp MTU Discovery
		+ Prototyp MTU Discovery dokumentieren
		+ Planung aktualisieren
		+ Meeting Open Systems AG abmachen