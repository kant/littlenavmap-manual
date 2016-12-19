# Änderungsprotokoll

## Änderungen von Version 1.0.5 zu 1.2

**Das Programm ist nicht mehr mit Windows XP kompatibel.**

_**Little Navconnect**_** wird nur noch für Netzwerkverbindungen gebraucht.**

### Neue Funktionen

#### Allgemein

* **Die Karte, der Flugplan, sowie Wetter- und Flugplatzinformationen können nun ausgedruckt werden.**
* **Nachtmodus und weitere Stile für die graphische Benutzeroberfläche hinzugefügt. Die Karte kann im Nachtmodus stufenweise abgedunkelt werden.**
* **Maßeinheiten können nun zwischen metrisch, imperial and nautisch separat für Distanz, Höhe, Geschwindigkeit, Gewicht und Volument eingestellt werden.**
* **Navigationsdatenaktualisierungen von **[**fsAerodata**](https://www.fsaerodata.com)** werden unterstützt.**
* Das Koordinatenformat kann nun zwischen Grad/Minuten/Sekunden und Dezimalformat umgeschaltet werden.
* Funkfrequenzen für VOR, NDB und ILS werden nun im Informationsfenster im Tab `Approaches` \(Anflugprozeduren\) angezeigt.
* Helikopterlandeplätze werden im Informationsfenster angezeigt.
* Das Programm zeigt nun optional den `Save as` \(Speichern als\) Dialog an, wenn Start-, Zielflugplatz oder der Flugplantyp geändert wurden. Dies vermeidet das Überschreiben von Flugplänen mit falschem Inhalt.
* Die aktuelle Kartenansicht kann als Bild abgespeichert werden.
* Hilfe ist nun entwerder offline als PDF-Datei oder online über Gitbook verfügbar.

#### Flugplan

* **Flugpläne können nun im GFP-Format exportiert werden, das von den Flight1 GTN 650/750 GPS-Systemen benutzt wird.**
* Benutzerdefinierte Wegpunkte können nun umbenannt werden.
* **ATS Routenbeschreibungen für Flugpläne können nun eingelesen und ausgegeben werden. Dabeit werden sogar Geschwindigkeit und Reisfughöhe erkannt.**
* Der aktive Flugplanabschnitt wird in der Flugplantabelle und auf der Karte hervorgehoben.
* Die Reiseflughöhe kann nun automatisch nach einer vereinfachten Ost/West Regel und den Flugplantype \(IFR oder VFR\) eingestellt werden.
* Reichweitenspalte für Funkfeuer in der Flugplantabelle hinzugefügt.

#### Wetter

* **Wetterdaten können nun direkt vom Simulator geholt werden und werden alle 15 Sekunden angezeigt. Diese Funktion steht auch für Netzwerkverbindungen zur Verfügung.**
* **Wetterdaten können nun im dekodierten Format für alle Quellen, wie Simulator, ASN, AS16, NOAA und Vatsim angezeigt werden.**
* Aus Active Sky kann nun das Flugplanwetter für Start- und Zielflugplatz auch in dekodiertem Format angezeigt werden. Dies ergibt präzise Wetterinformationenfür ASN oder AS16 Benutzer.
* Zeiger am oberen Rand der Karte für den Wind um das Nutzerflugzeug hinzugefügt.

#### Kartendarstellung

* **AI- und Multiplayer-Flugzeuge werden nun auf der Karte angezeigt. Informationen werden nach Anklicken im `Aircraft Progress Window` und in Tooltips angezeigt.**
* **Ein konfigurierbare Anzeige für den Start des Sinkfluges zum Ziel wurde hinzugefügt. Die Anzeige basiert auf der einfachen 3 nautische Meilen pro 1000 Fuß Regel.**
* Die Steuerungselemente der Karte können nun deaktiviert werden.
* Ein neuer optionaler Modus rollt die Karte nun kontinuierlich um den Benutzerflugzeug zu folgen.
* Die Bewegungen des Benutzer, sowie der AI- bzw. Multiplayer-Flugzeuge sind nun flüssiger.
* Das Symbol der Benutzerflugzeuges kann nun optional eine Linie zu Darstellung der Bewegungsspur angezeigt werden.
* Flugzeugtypen, wie Jet, Kolbenmotor bzw. Turboprop und Helikopter werden über das Flugzeugsymbol angezeigt.
* Die minimale sicher Flughöhe wird jetzt für alle Flugplansegmente im Höhenprofil angezeigt.
* Die Landebahnlänge wird nun in genauen Einheiten, wie Meter oder Fuß abhängig von den eingestellten Maßeinheiten angezeigt.
TODO
* **Die Texte für Flugplätze, Benutzer- und AI- bzw. Multiplayer-Flugzeuge können separat geändert werden.**
* **Symbol- und Textgrößen für Flugplätze, Navigationspunke, Benutzer- und AI- bzw. Multiplayer-Flugzeuge können einzeln geändert werden.**
* Die Line der Benutzerflugzeugspur kann nun in Breite, Farbe und Typ geändert werden.
* Die Linienbreite von Enternungsringen und Distanzmesslinien kann geändert werden.
* Die Zoomentfernung für Doppelklick und `Show on map` Menüpunkte kann einzeln eingestellt werden.
* Beim Programmstart kann nun optional die letzte Route auf der Karte zentriert werden.

#### Verbindung zum Flugsimulator

* _**Little Navmap**_** kann sich nun direkt mit dem Flugsimulator verbinden. **_**Little Navconnect**_** wird nur noch für Netzwerkverbindungen benötigt.**
* _**Little Navmap**_** kann nun optional automatisch die Verbindung zum Simulator oder einer entfernten Instanz von **_**Little Navconnect**_** aufbauen. Die Startreihenfolge der Programme ist nun irrelevant.**
* Rechnernamen und IP-Adressen können im Dialog `Connect` aus der Liste gelöscht werden.

### Problembeseitigungen

#### Allgemein

* **Die OpenTopoMap ist wieder zurück in ihrer vollen Pracht. Sämtliche Karten, die HTTPS benötigen funktionieren nun wieder korrekt.**
* **Der Kurs zu oder von benutzerdefinierten Wegpunkten war unter bestimmten Bedingungen falsch, da die magnetische Varianz nicht richtig ausgewertet wurde.**
* **Die Flugplanberechnung stürzt nun nicht mehr ab, wenn die Navigationsdaten von **[**FSX/P3D Navaids update**](http://www.aero.sors.fr/navaids3.html)** benutzt werden.**
* Die Flugplanberechnung spring nun nicht mehr zwischen verschiedenen Luftstraßen.
* Die Zeilenenden für gespeicherte PLN-Dateien werden nun immer im Windows-Format geschrieben, um das Laden in PF3 ATC zu ermöglichen.
* Der Routentyp von Flugplänen war unter Umständen leer, wenn ein Flugplan gespeichert wurde. Der Simulator konnte dies Flugpläne nicht laden.
* Die magnetische Varianz wurden manchmal in Tooltips und im Informationsfenster falsch dargestellt.
* Ein altes Problem, das dazu führte, dass Tooltips willkürlich wieder auftauchten wurde beseitigt.

#### Szeneriedatenbank

* Problemumgehung für zu lange Luftstraßensegmente hinzugefügt. Diese werden nun beim Laden ausgelassen.
* Fixed problem when reading too small BGL files into the scenery database.
* Zoomproblem mit bestimmten Add-on Flugplätzen beseitigt, die eine weit entfernte Landebahnatrappe enthalten. Alle Landebahnen, die mehr als 50 Kilometer vom Flugplatz entfernt sind werden nun ausgelassen.
* Luftraßen werden nun nicht mehr in unnötig viele Fragmente aufgespalten.
* Ein Problem wurde beseitigt, das zu viele Landebahnoberfläschen als ungültig \(`invalid.`\) markier hatte.

