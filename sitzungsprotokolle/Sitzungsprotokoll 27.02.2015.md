###Zweites Meeting 13:00 - 27.02.2015 (KW9)  
**Teilnehmer:** Andreas Steffen, Tobias Brunner, Stefan Keller (Open Systems), James Hulka (Open Systems), Jan Balmer, Theo Winter

+ Herr Steffen hat noch Bedenken bezüglich der Performance von Java. Wir sollen deshalb eine Risiko-Analyse vorziehen und Performance Tests machen. Unser Tool soll in der Lage sein mindestens 20mbit/s an Traffic aufzuzeichnen. Gem. Open Systems kann es zu Peaks von bis zu 300mbit/s kommen, diese sind aber eher selten.

+ Auf einem Node kann es mehrere Tunnels haben, unser Tool soll die Pakete von allen Tunnels abfangen. Es kann ausserdem sein das es z.B. 2 Routen zum selben Node geben kann.

+ Es ist möglich Open Systems zu besuchen und dort z.B. die MTU and Live Daten zu messen.

+ Unser Tool wird auf beiden Seiten des Tunnels laufen, d.h. wir können selbst Pakete durch schicken und diese auf der anderen Seite wieder empfangen. Von unserem Tool soll es nur eine Ausführung geben, d.h. nicht ein Client-Server.

+ Die Dokumentation wird auf Deutsch sein, wir werden jedoch ein kurzes User-Handbuch auf Englisch verfassen.

+ Eine Alternative zu libpcap wäre noch goprobe. Empfohlen von J. Hulka.

+ Um Tests durchzuführen wird uns ein Testaufbau mit VMs in VirtualBox empfohlen, wie wir virtuelle Router erstellen können müssen wir noch rausfinden. --> J. Balmer kümmert sich darum.

+ Die Ausgabe des Tools soll die Information sein, viele % der Pakete gedroppt werden, wenn ein Schwellwert überschritten wird soll ein Alert ausgeführt werden. Open Systems hat entsprechende Systeme die diesen Alert dann aufnehmen würden.

+ Die Tunnels von Open Systems laufen im Transport Mode.

+ Optional könnte man noch passiv die IKE Header untersuchen. (UC4)

+ Idealerweise benötigt das Tool möglichst wenig statische Konfiguration und kann möglichst viele Informationen automatisch beziehen, der Einfachheit halber werden wir aber mit einem config file beginnen wo z.B. src und dest IP drin stehen.

+ Das Tool soll die MTU Tests periodisch & automatisch durchführen. Dies lässt sich entweder via selbst gebautem Daemon realisieren oder via Cronjob.

+ Ansprechpartner bei Open Systems sind Stefan Keller (sk @ open.ch) und James Hulka (jah @ open.ch).

+ Wir werden ca. in der Mitte des Projekts ein weiteres Meeting mit Open Systems AG haben wo wir noch Architektur Details besprechen können und den aktuellen Prototyp zeigen. Dieses Meeting wird ca. in der 5-6 Woche des Projekts stattfinden.