_Woraus besteht ein Computernetzwerk?_
___
### Bestandteile:

- Übertragungsmedien (Kabel, Funk, …)
- Aktive Komponenten:
    - Hub
    - Switch
    - Router
    - Layer 3 Switch bzw. Layer 4 Switch
    - Gateway
    - Access Point
### 7-Schichtenmodell und Komponenten:

|Schicht|Name|Komponente|
|---|---|---|
|7|Anwendungsschicht||
|6|Präsentationsschicht||
|5|Kommunikationsschicht||
|4|Transportschicht|Layer 4 Switch, Gateway|
|3|Vermittlungsschicht|Router, Layer 3 Switch|
|2|Sicherungsschicht|Switch, Access Point|
|1|Übertragungsschicht|Verkabelung / Hub|

### Hub:

- Einfacher Verteiler
- Verteilt Datenpakete an alle Hosts
- Vorteile: Günstig, einfache Bauweise
- Nachteile: Enormer Datenverkehr, eventueller Datenverlust
### Switch:

- Ordnet Datenpakete den einzelnen Empfängern zu
- Zuordnung anhand der MAC Adresse
- Vorteile: Verhinderung von Datenverlust, schneller als Hub
- Nachteile: Teurer als Hub, begrenzte Anzahl gespeicherter MAC Adressen
### MAC Adresse:

- Jede Netzwerkhardware hat eine eingelötete Adresse
- Ein Gerät kann mehrere MAC Adressen haben (z.B. für Ethernet und WLAN)
- Kann in der Commandline mit "ipconfig/all" ausgelesen werden
- Wird als "physikalische Adresse" angezeigt
### Router

- Verbindet mehrere Netzwerke mit dem gleichen Protokoll miteinander
- Z.B.: das eigene LAN mit dem Internet
- Befindet sich in der Regel an der Außengrenze des Netzwerks
- Reagiert selbstständig auf Ausfälle
- Verbindet LAN und WAN
### Layer 3 Switch

- Mischung aus Switch und Router (auch Router-Switch genannt)
- Vorteile gegenüber Router:
    - Geringere Verzögerungszeit
    - Einfachere Administration
- Nachteil gegenüber reinem Router:
    - Weniger Funktionen
### Layer 4 Switch

- Ähnlich wie Layer 3 Switch, kann aber auch Transportprotokolle erkennen
- Große Datenmengen (z.B. Videos) werden mittels UDP übertragen (schnell, aber mit eventuellem Datenverlust)
- Kleinere Datenmengen oder wichtige Daten werden mittels TCP übertragen (langsamer, aber sicher)
### Gateway

- Verbindet mehrere physikalisch zueinander inkompatible Netzwerke
- Beispiele: Verbindung vom LAN zum Faxgerät oder Voice over IP vom PC auf das Festnetztelefon
### Access Point

- Ermöglicht Zugriff aufs lokale Netzwerk mittels WLAN
- Nicht zu verwechseln mit einem Range Extender
- Range Extender empfängt und verstärkt WLAN-Signale
- Access Point empfängt WLAN-Signal und gibt es im LAN weiter
- Funktioniert in beide Richtungen