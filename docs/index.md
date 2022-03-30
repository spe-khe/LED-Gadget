# SPE Karlsruhe - MultiMonG
{:toc}
## Vorwort
Dieses Dokument ist in mehreren Kapiteln gegliedert und soll dir das Gadget (Multi-Monitoring Gadget) näherbringen. Darum wird im ersten Kapitel das Gadget im Allgemeinen vorgestellt. Hierzu gehören die verschiedenen Funktionen und der Mikrocontroller. Im nächsten Kapitel wird auf die Module, den Verdrahtungsplan, und die Bauteile des Gadgets eingegangen. Damit im darauffolgenden Kapitel, mit der Inbetriebnahme des Gadgets angefangen werden kann. Im vorletzten Kapitel wird die Programmierung vorgestellt und schematisch an einem Beispiel erklärt. Daraufhin folgt eine Anleitung, in der beschrieben wird, wie du dein Gadget programmieren kannst. Zum Schluss folgt das letzte Kapitel, indem der Ablauf der Konstruktion und die Planung deines Gadgets vorgestellt wird.

## Einführung
Das Gadget ist eine Station mit insgesamt sieben Funktionen. Diese Funktionen werden mit einem Mikrokontroller und verschiedenen Modulen realisiert. Diese Funktionen sind:
1. Anzeigen der aktuellen Uhrzeit
2. Anzeigen der Temperatur
3. Anzeigen der Luftfeuchte
4. Anzeigen des Timers
5. Anzeigen einer eigenen Nachricht
6. Anzeigen der Luftqualität
7. Zyklisches wechseln (5 Sekunden), zwischen Funktion eins, zwei, drei und sechs

Auf die Funktionen wird in den nächsten Kapiteln ausführlicher eingegangen.
Ein Mikrocontroller ist ein „kleiner mini Computer“. Sie sind im Alltag eher unbekannt und
sind die Helden hinter den Dingen. Viele Geräte wären ohne einen Mikrocontroller undenkbar. Meistens werden sie für Steuerungs- und Kommunikationsaufgabe eingesetzt. So finden sie z.B. in den folgenden Geräten und Anwendungen ihren Platz:
* Radio
* Roboter
* Fernseher
* Flugzeuge
* Fernbedienungen
* Waschmaschinen
* Intelligente Systeme z.B. Airbag
* Intelligente Systeme in der Automatisierung
* Erfassung von Messwerten z.B. Drehzahl

Die Aufgaben sind vielfältig und so auch die Möglichkeiten, die sich dadurch ergeben. Ein Mikrocontroller muss für seine zu bewerkstelligende Aufgabe programmiert werden. Diesen Programmcode durchläuft der Mikrocontroller immer wieder „unendlich oft“. So führt er präzise seine Aufgabe aus und kommt dabei nicht durcheinander, denn er führt Zeile für Zeile in seinem programmierten Code aus. Dadurch wird auch deutlich, dass die Programmierung ein wesentlicher Bestandteil der Elektrotechnik ist und immer mehr Einzug erhält.

![ESP8266](docs/assets/images/ESP8266.jpg)

## Aufbau
Insgesamt besteht das Gadget aus den folgenden acht Bauteilen:
* Platine 		
* Holzbrett 	
* Taster 		
* Lautsprecher 	
* Steckleiste 	
* ESP8266 
* DHT11 (Sensor) 
* Verbinder 
* MQ135 (Luftqualitätssensor) 
* LED-Matrix

<div class="flex-container" style="margin: 1em">
        <img src="docs/assets/images/Platine.png" style="height: 10em">
        <img src="docs/assets/images/Holzbrett.png" style="height: 10em">
        <img src="docs/assets/images/Taster.png" style="height: 10em">
        <img src="docs/assets/images/Buzzer.png" style="height: 10em">
        <img src="docs/assets/images/Steckleisten.png" style="height: 10em">
        <img src="docs/assets/images/Winkel.png" style="height: 10em">
        <img src="docs/assets/images/ESP8266.jpg" style="height: 10em">
        <img src="docs/assets/images/DHT11.png" style="height: 10em">
        <img src="docs/assets/images/Verbinder.png" style="height: 10em">
        <img src="docs/assets/images/MQ135.png" style="height: 10em">
        <img src="docs/assets/images/Matrix.png" style="height: 10em">
</div>

Diese Bauteile müssen korrekt verdrahtet bzw. miteinander verbunden werden, damit die entsprechenden Funktionen gegeben sind. Diese Aufgabe übernimmt die Platine für uns. Auf ihr befinden sich Leiterbahnen, die die Verbindungen zwischen den Modulen und dem Mikrocontroller herstellen.
In der folgenden Abbildung ist der Schaltplan eures Gadgets zu sehen. Es fällt auf, dass jedes Bauteil  seinen eigenen Steckplatz hat. Die Größe der Bauteile sind auf der Platine angedeutet und  müssen korrekt gesteckt, sowie verlötet werden.
Hierbei ist es wichtig auf die Polarität der Bauteile zu achten, und auf eine angemessene Verlötung Wert zu legen, damit jede Verbindung korrekt verbunden ist.
![Schaltplan](docs/assets/images/Schaltplan.png)


