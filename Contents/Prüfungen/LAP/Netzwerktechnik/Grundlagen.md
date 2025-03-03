---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/Grundlagen.md
---

## **Was ist eine IP-Adresse?**

Eine IP-Adresse (Internet Protocol Address) ist eine eindeutige numerische Kennung, die jedem Gerät in einem Netzwerk zugewiesen wird. Sie ermöglicht die Identifikation und Kommunikation zwischen Geräten im Internet oder lokalen Netzwerken. Es gibt zwei Versionen: IPv4 (z. B. 192.168.1.1) und IPv6 (z. B. 2001:0db8::1).

## **Erklären Sie den Begriff „MAC-Adresse“.**

Eine MAC-Adresse (Media Access Control Address) ist eine einmalige physische Adresse, die einer Netzwerkschnittstelle zugewiesen ist. Sie dient der Identifikation von Geräten im lokalen Netzwerk und wird in der Regel in der Hardware (z. B. Netzwerkkarte) festgelegt. Eine MAC-Adresse besteht aus 48 Bit und wird in Form von Hexadezimalzahlen dargestellt, z. B. 00:1A:2B:3C:4D:5E.

## **Erklären Sie den Unterschied zwischen einer v4 und v6 IP-Adresse.**

Eine IPv4-Adresse besteht aus 32 Bit und wird in vier Dezimalzahlen dargestellt, z. B. 192.168.0.1. Sie ermöglicht etwa 4,3 Milliarden eindeutige Adressen.

Eine IPv6-Adresse besteht aus 128 Bit und wird in acht Hexadezimalblöcken dargestellt, z. B. 2001:0db8::1. Sie bietet eine nahezu unbegrenzte Anzahl an Adressen und löst das Adressmangelproblem von IPv4.

## **Erklären Sie den Aufbau einer IPv4-Adresse.**

Eine IPv4-Adresse besteht aus 32 Bit und wird in vier Dezimalzahlen dargestellt, die jeweils durch Punkte getrennt sind (z. B. 192.168.1.1). Jede Dezimalzahl repräsentiert 8 Bit (ein Oktett) und hat einen Wertebereich von 0 bis 255.

### IPv4 Aufbau

**Netzwerkanteil**
Identifiziert das Netzwerk, zu dem das Gerät gehört.

**Hostanteil**
Identifiziert das Gerät innerhalb des Netzwerks.

> [!INFO] Der Anteil von Netzwerk und Host wird durch die Subnetzmaske festgelegt. Beispiel: Bei der Subnetzmaske 255.255.255.0 gehört der erste Teil (192.168.20) zum Netzwerk, während die letzte Zahl (1) den Host darstellt.
$$Netzwerk = 192.168.20.xx/24$$
> $$Host = xx.xx.xx.1-254$$  

## **Erklären Sie den Aufbau einer IPv6-Adresse.**

Eine IPv6-Adresse besteht aus 128 Bit und wird in acht Gruppen von jeweils 16 Bit unterteilt. Jede Gruppe wird durch einen Doppelpunkt getrennt und in hexadezimaler Schreibweise dargestellt.

### Aufbau einer IPv6-Adresse

- Gesamtlänge: 128 Bit
- Unterteilung: 8 Gruppen à 16 Bit
- Darstellung: Hexadezimale Schreibweise (0-9 und A-F)
- Trennzeichen: Doppelpunkt zwischen den Gruppen

### Beispiel einer vollständigen IPv6-Adresse

``` HEX
FE80:CD00:0000:0CDE:1257:0000:211E:029C
```

### Kurzschreibweisen zur Vereinfachung

- Weglassen führender Nullen in jeder Gruppe
- Ersetzen aufeinanderfolgender Nullgruppen durch "::" (einmalig pro Adresse)

> [!EXAMPLE] Verkürzte Beispieladresse
FE80:CD00::CDE:1257:0:211E:29C

### IPv6 Aufbau

**Netzwerkteil (Network Prefix): Die ersten 64 Bit **
 - Routing-Präfix
- Subnetz-ID

**Knotenteil (Interface Identifier): Die letzten 64 Bit **
 - Identifiziert die Netzwerkschnittstelle

> [!INFO] Diese Struktur ermöglicht eine flexible Adressierung und vereinfacht das Routing im IPv6-Netzwerk

## **Erklären Sie den Begriff „Netzwerkmaske bzw. Subnetzmaske“.**

Die Netzwerkmaske oder Subnetzmaske ist ein grundlegendes Konzept in der Netzwerktechnik, das verwendet wird, um eine IP-Adresse in zwei Teile zu unterteilen: den Netzwerkanteil und den Hostanteil. Sie ist eine Bitmaske, die festlegt, welche Bits einer IP-Adresse den Netzwerkbereich und welche den Hostbereich repräsentieren. 

### Aufbau und Funktion

- Die Subnetzmaske besteht aus einer Reihe von 1-Bits (für den Netzwerkanteil) gefolgt von 0-Bits (für den Hostanteil).
- Sie wird in IPv4-Netzen als 32-Bit-Wert dargestellt, z. B. 255.255.255.0.
- In IPv6 wird die Präfixlänge (z. B. /64) verwendet, die die Anzahl der Bits für den Netzwerkanteil angibt.

> [!INFO] Die Subnetzmaske ist essenziell für Routing und Adressierung in Netzwerken und wird häufig bei der Konfiguration von Netzwerken verwendet, um Datenverkehr effizient zu steuern und zu segmentieren.

## **Erklären Sie den Begriff „CIDR (Classless Inter-Domain Routing)“.**

CIDR (Classless Inter-Domain Routing) ist eine Methode zur flexiblen Zuweisung und effizienten Verwaltung von IP-Adressen im Internet. Es wurde 1993 eingeführt, um zwei Hauptprobleme zu lösen: die Knappheit von IPv4-Adressen und die Überlastung der Routing-Tabellen.

Sprich die Slash Notation von Netzwerkmasken. Ermöglicht Netze noch kleiner aufzuteilen.

### Beispiel
Network        = 10.1.152.0 / 26
Netmask        = 255.255.255.192
Broadcast      = 10.1.152.63
Wildcard Mask  = 0.0.0.63
Max. Hosts     = 62   (2^6 - 2)
Host Range     = { 10.1.152.1 - 10.1.152.62 }

### Merkmale von CIDR

**Flexible Adresszuweisung**
CIDR ermöglicht eine effizientere Nutzung des IP-Adressraums, indem es die starren Grenzen der klassischen Netzklassen (A, B, C) aufhebt. 

**Präfix-Notation**
Eine CIDR-Adresse wird als IP-Adresse gefolgt von einem Schrägstrich und der Präfixlänge angegeben, z.B. 192.168.1.0/24. 

**Subnetting und Supernetting**
CIDR erlaubt die Unterteilung großer Netzwerke in kleinere Subnetze oder die Zusammenfassung mehrerer kleiner Netzwerke zu einem größeren. 

**Reduzierung der Routing-Tabellen**
Durch die Aggregation von Adressbereichen werden die Routing-Tabellen im Internet-Backbone verkleinert, was das Routing effizienter macht. 

**Verwendung einer Subnetzmaske variabler Länge (VLSM)**
Dies ermöglicht eine flexiblere Aufteilung des Adressraums.

> [!INFO] CIDR hat die IP-Adressverwaltung revolutioniert und ist heute der Standard für IP-Adresszuweisung und Routing im Internet. Es dient als Zwischenlösung bei der Umstellung von IPv4 auf IPv6, indem es die Lebensdauer des IPv4-Adressraums verlängert

## **Erklären Sie den Begriff „Broadcast-Adresse“.**

Die Broadcast-Adresse ist eine spezielle IP-Adresse, die verwendet wird, um Datenpakete an alle Geräte in einem bestimmten Netzwerk oder Subnetz zu senden.

### Wesentliche Merkmale der Broadcast-Adresse sind

- Sie ist die letzte IP-Adresse eines Subnetzes.
- Sie wird genutzt, um Informationen an alle Teilnehmer eines Netzwerks zu übertragen, ohne deren individuelle IP-Adressen zu kennen.
- In IPv4-Netzwerken sind alle Host-Bits der Adresse auf 1 gesetzt.
- Sie ermöglicht es Netzwerkadministratoren, die erfolgreiche Übermittlung von Datenpaketen zu überprüfen.

### Es gibt zwei Arten von Broadcasts

**Limited Broadcast**
Verwendet die IP-Adresse 255.255.255.255 und zielt auf alle Geräte im lokalen Netz.

**Directed Broadcast**
Adressiert alle Empfänger innerhalb eines bestimmten Netzes und kombiniert die IP-Adresse des Zielnetzwerks mit dem Setzen aller Hostbits auf 1.

> [!INFO] Die Broadcast-Adresse spielt eine wichtige Rolle bei der Netzwerkkommunikation, insbesondere für Dienste wie DHCP und ARP, die alle Geräte in einem Netzwerk erreichen müssen

**Erklären Sie den Begriff „Multicast-Adresse“.**

Eine Multicast-Adresse ist eine spezielle IP-Adresse, die verwendet wird, um Datenpakete gleichzeitig an eine Gruppe von Empfängern in einem Netzwerk zu senden.

## **Wesentliche Merkmale der Multicast-Adresse sind:**

- Sie ermöglicht die effiziente Übertragung von Daten an mehrere Empfänger, ohne die Netzwerklast zu erhöhen.
- In IPv4 liegt der Adressbereich für Multicast zwischen 224.0.0.0 und 239.255.255.255
- In IPv6 beginnen Multicast-Adressen mit dem Präfix FF00::/8.
- Multicast-Adressen definieren Empfängergruppen, die sich für bestimmte Datenströme registriert haben.
- Sie wird in verschiedenen Anwendungsbereichen eingesetzt, wie Streaming von Multimedia-Inhalten, Echtzeitdatenübertragungen und Softwareverteilung.

 > [!INFO]  Multicast-Adressen ermöglichen es einem Sender, eine einzelne Kopie der Daten zu versenden, die dann effizient an alle Mitglieder der Multicast-Gruppe verteilt wird. Dies unterscheidet sich von Unicast, bei dem Daten einzeln an jeden Empfänger gesendet werden, und von Broadcast, bei dem Daten an alle Netzwerkteilnehmer gesendet werden

## **Erklären Sie den Begriff „ARP-Protokoll“ und seine Funktion.**

Das ARP-Protokoll (Address Resolution Protocol) ist ein Netzwerkprotokoll, das in lokalen Netzwerken (LANs) verwendet wird, um IP-Adressen in MAC-Adressen umzuwandeln. Seine Hauptfunktionen sind:

**Adressauflösung**
ARP ermöglicht die Zuordnung von IP-Adressen zu physischen MAC-Adressen von Netzwerkgeräten. 

**Kommunikationsermöglichung**
Es ermöglicht die Datenübertragung auf der Ethernet-Ebene, indem es die physische Adresse des Zielgeräts identifiziert. 

**Netzwerkeffizienz**
ARP verwendet einen Cache (ARP-Cache), um kürzlich aufgelöste IP-MAC-Zuordnungen zu speichern, was die Anzahl der ARP-Anfragen reduziert und die Netzwerkleistung verbessert. 

**Broadcast-Anfragen**
Wenn eine MAC-Adresse nicht im Cache gefunden wird, sendet ARP eine Broadcast-Anfrage an alle Geräte im Netzwerk. 

**IPv4-Spezifisch**
ARP wird hauptsächlich in IPv4-Netzwerken verwendet. In IPv6-Netzwerken übernimmt das Neighbor Discovery Protocol (NDP) diese Funktion.

> [!INFO] ARP spielt eine entscheidende Rolle bei der effizienten Datenübertragung in Ethernet-Netzwerken, indem es die Lücke zwischen der Netzwerkschicht (IP) und der Datenverbindungsschicht (MAC) überbrückt

## **Erklären Sie den Begriff „ICMP-Protokoll“ und seine Funktion.**

Das ICMP-Protokoll (Internet Control Message Protocol) ist ein Netzwerkprotokoll, das für die Übermittlung von Steuerungs- und Fehlermeldungen in IP-Netzwerken verantwortlich ist. 

### Hauptfunktionen

**Fehlererkennung und -meldung**
ICMP ermöglicht es Netzwerkkomponenten, Fehler zu erkennen und Fehlermeldungen an den Absender zu senden. 

**Zustandsinformationen**
Es erlaubt Netzwerkgeräten, Statusinformationen über andere Komponenten abzurufen. 

**Netzwerkdiagnose**
ICMP wird für Tools wie Ping verwendet, um die Erreichbarkeit und Latenz von Netzwerkzielen zu überprüfen. 

**Router-Kommunikation**
Es erleichtert den Informationsaustausch zwischen Routern über den Netzwerkzustand.
  
> [!NOTE]
ICMP arbeitet auf der Netzwerkschicht des TCP/IP-Modells und verwendet IP-Pakete für die Übertragung seiner Nachrichten. Es ist ein unzuverlässiges Protokoll, da ICMP-Nachrichten ohne Bestätigung gesendet werden und im Netzwerk verloren gehen können.
>
Zwei häufig genutzte ICMP-Nachrichtentypen sind der Echo Request und der Echo Reply, die die Grundlage für das Ping-Tool bilden. ICMP spielt eine wichtige Rolle bei der Aufrechterhaltung und Diagnose von Netzwerken, indem es Probleme identifiziert und meldet, was zur Effizienzsteigerung in modernen Netzwerken beiträgt

## **Erklären Sie den Begriff „Frame“.**

Ein Frame in der IT ist eine strukturierte Dateneinheit, die für die Übertragung von Informationen in Netzwerken verwendet wird. Frames spielen eine wichtige Rolle auf der Datenverbindungsschicht (Schicht 2) des OSI-Modells.

### Hauptmerkmale eines Frames

**Größe**
Typischerweise zwischen 64 und 1518 Bytes, abhängig vom Netzwerkprotokoll

**Struktur**
Besteht aus Header, Nutzdaten und Trailer

**Funktion**
Trägt Daten und steuert die korrekte Übermittlung im Netzwerk

### Bestandteile eines Frames

**Header**
- Ziel- und Quellenadressen (MAC-Adressen)
- Steuerinformationen

**Nutzdaten**
 - Die eigentlichen zu übertragenden Daten

**Trailer**
- Prüfsumme zur Fehlererkennung (Frame Check Sequence)

### Bedeutung in verschiedenen Kontexten

**Ethernet**
Grundlegende Dateneinheit in Ethernet-Netzwerken

**Paketbasierte Netzwerke**
Container für einzelne Netzwerkpakete

**Zeitmultiplexverfahren**
Zyklisch wiederholter Datenblock mit fester Anzahl von Zeitschlitzen

> [!NOTE]
> Frames ermöglichen eine effiziente und zuverlässige Datenübertragung, indem sie die zu sendenden Informationen strukturieren und mit wichtigen Metadaten versehen. Sie sind entscheidend für die korrekte Interpretation, Zuordnung und Fehlerüberprüfung von Daten durch Netzwerkgeräte wie Computer, Switches und Router

## **Erklären Sie den Begriff „Port-Forwarding“ und für was es eingesetzt wird.**

Port-Forwarding ist eine Technik, bei der Datenpakete von einem Router-Port an ein bestimmtes Gerät im lokalen Netzwerk weitergeleitet werden. 

### Hauptzwecke

- Zugriff auf interne Server von außen
- Fernsteuerung von Geräten
- Ermöglichen von Online-Spielen
- VPN-Verbindungen

### Funktionsweise
Router leitet externe Anfragen an definierte interne Geräte weiter mit Network Address Translation (NAT)

**SNAT**
Privat auf Öffentlich (Router zu Hause)

**DNAT**
Öffentlich auf Privat (wenn ich zu hause hinter einer Öffentlichen IP einen Server Hosten möchte)

**PAT (Port Address Translation)**
hier gebe ich ausschließlich bestimmte Ports frei für den Traffic.

> [!NOTE]
Bei SNAT und DNAT werden die IP´s geNATet. Bei PAT die Ports selber!

 > [!CAUTION] Sicherheitshinweis
> - Nur notwendige Ports öffnen
> - Firewall und Passwörter nutzen
