###Sechstes Meeting 13:00 - 28.03.2015 (KW13)  
**Teilnehmer:** Tobias Brunner, Jan Balmer, Theo Winter

+ **Aktueller Stand gezeigt:**
	+ MTU Discovery Prototyp gezeigt, senden empfange via localhost geht.
	+ Vom Packet loss prototyp erzählt.
	
+ **MTU Discovery:** T. Brunner hatte noch ein paar Tipps: Wir sollen Paket gleicher Grösse auch zurücksenden nicht nur kleines "ok" Paket da evtl. beim Rückweg eine andere Route genommen wird. Und anstelle mehrere Durchgänge mit einem fixen MTU-Erhöhungsschritt könnten wir auch jeweils mit der halben Erhöhungsgrösse schaffen. D.h. wenn wir z.B. normal die Paketgrösse um 100Bytes erhöhen und so an ein Limit kommen gehen wir zurück zur letzten erfolgreichen Grösse und erhöhen um 50Bytes.

+ **Meeting Open Systems AG:** Ich habe das Meeting mit Open Systems diese Woche organisiert. T.Brunner sagt dies ist gut so, den Raum müssen wir nicht reservieren dass wir von A.Steffen übernommen oder aber wir nehmen einfach den Tisch im ITA Zimmer, wir müssen uns nicht darum kümmern.

+ **Packet loss:** T.Brunner hat J.Balmer noch ein paar Tipps zum Paket-Verlust messen gegeben. Unter anderem ist die Default-Window Size 32. Open Systems arbeitet aber mit einer Window-Size von 512. Pakete die ausserhalb das Window fallen werden ja verworfen, es könnte aber interessant sein diese trotzdem in die Paket-Verlust Messung mit einzubeziehen weil man dann sieht das die Pakete doch noch angekommen sind, einfach verspätet.
	
+ **Nächstes Meeting:** Nur mit T.Brunner weil A.Steffen weg ist. Es findet nächsten Donnerstag um 11:00 statt weil darauf Karfreitag ist.

+ **Weiteres Vorgehen:**

	+ **Jan:**
		+ VMs fertig dokumentieren (Text zu Bild)
		+ Prototyp Paketverlust weiterprogrammieren, fortlaufend dokumentieren
		+ NFRs überarbeiten
		
	+ **Theo:**
		+ Prototyp verbessern, fortlaufend dokumentieren
		+ Risiken in Doku erweitern