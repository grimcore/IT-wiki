---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/Routing.md
sticker: lucide//book-open-check
---

## Was ist eine „Routing Tabelle“?

Eine Routing-Tabelle ist eine Datenstruktur, die von Netzwerkgeräten wie Routern verwendet wird, um Entscheidungen über die Weiterleitung von Datenpaketen zu treffen. Sie enthält wichtige Informationen für das effiziente Routing in Netzwerken.

### Zieladresse/IP-Adressbereich
Gibt an, für welches Zielnetz der Eintrag gilt.

### Nächster Hop / Gateway
Zeigt das nächste Zwischenziel auf dem Weg zum Ziel an.

### Interface
Gibt die physische oder logische Schnittstelle an, über die das Paket gesendet wird.

### Metrik
Bestimmt die Qualität einer Route, oft basierend auf der Anzahl der Zwischenstationen oder der geschätzten Zeit.

> [!note]
Router konsultieren ihre Routing-Tabellen Millionen Mal pro Sekunde, um den Netzwerk-Traffic zu bewältigen und die besten Wege für Datenpakete zu finden. Die Tabelle hilft dabei, den effizientesten Pfad für die Datenübertragung von der Quelle zum Ziel zu bestimmen. Routing-Tabellen spielen eine zentrale Rolle bei der Effizienz und Sicherheit von Netzwerkinfrastrukturen, indem sie die Regeln für den Datentransport zwischen Netzwerken, Routern und Endgeräten festlegen

## Was ist eine „Default Route“?

Eine Default Route, auch als Standard-Route bezeichnet, ist ein spezieller Eintrag in der Routing-Tabelle eines Netzwerkgeräts, der für die Weiterleitung von Datenpaketen verwendet wird, wenn keine spezifische Route für das Ziel gefunden wurde.

### Hauptmerkmale der Default Route

- Wird als 0.0.0.0/0 in IPv4 oder ::/0 in IPv6 dargestellt
- Dient als "Auffangroute" für alle nicht anderweitig zugeordneten Ziele
- Leitet Pakete typischerweise zum nächsten Router oder zum Internet-Gateway weiter
- Hat in der Regel eine niedrigere Priorität als spezifischere Routen

### Die Default Route spielt eine wichtige Rolle in Netzwerken, da sie: 

- Die Weiterleitung von Paketen zu unbekannten Zielen ermöglicht
- Die Größe der Routing-Tabelle reduziert, indem nicht jedes mögliche Ziel einzeln eingetragen werden muss
- Oft auf den Router zeigt, der die Verbindung zum Internet-Service-Provider herstellt

> [!note]
In komplexeren Netzwerken können mehrere Default Routes mit unterschiedlichen Prioritäten konfiguriert werden, um Redundanz und Lastverteilung zu gewährleisten

## Was ist eine „Statische Route“?

Eine statische Route ist ein manuell konfigurierter Eintrag in der Routing-Tabelle eines Netzwerkgeräts, der den Pfad für die Weiterleitung von Datenpaketen zu einem bestimmten Zielnetzwerk festlegt. 

### Hauptmerkmale statischer Routen

- Werden vom Netzwerkadministrator manuell konfiguriert
- Bleiben unverändert, bis sie manuell geändert oder entfernt werden
- Eignen sich besonders für kleine, stabile Netzwerke mit wenigen Routen

### Vorteile

- Einfach zu konfigurieren und zu verstehen
- Volle Kontrolle über die Routen
- Keine zusätzliche CPU- und Speicherbelastung
- Weniger anfällig für bestimmte Netzwerkangriffe

### Nachteile

- Erfordern manuelle Wartung
- Nicht skalierbar für große Netzwerke
- Keine automatische Anpassung an Netzwerkänderungen
- Geringere Fehlertoleranz bei Ausfällen

> [!note]
Statische Routen werden oft in Situationen eingesetzt, wo eine präzise Steuerung des Datenverkehrs erforderlich ist, wie zur Optimierung des Datenverkehrs, Erhöhung der Netzwerksicherheit oder für Netzwerk-Debugging

## Was ist eine „Dynamische Route“?

Eine dynamische Route ist eine Methode zur automatischen Konfiguration und Aktualisierung von Routen in einem Netzwerk. 

### Hauptmerkmale dynamischer Routen

- Router verwenden Routing-Protokolle, um Routen automatisch zu lernen und zu aktualisieren.
- Sie passen sich Netzwerkänderungen wie Ausfällen oder neuen Netzwerken an.
- Routing-Tabellen werden automatisch aktualisiert, basierend auf Echtzeitänderungen der Netzwerkbedingungen.
- Mehrere mögliche Routen zum Ziel stehen zur Verfügung.
- Algorithmen werden verwendet, um den besten Weg für den Datenverkehr zu bestimmen.

### Vorteile dynamischer Routen

- Bessere Anpassungsfähigkeit an Netzwerkänderungen
- Höhere Skalierbarkeit, besonders in großen Netzwerken
- Automatische Umleitung des Datenverkehrs bei Ausfällen
- Effizientere Verwaltung in komplexen Netzwerken

> [!note]
Dynamische Routen werden häufig in größeren, sich häufig ändernden Netzwerken eingesetzt, wo manuelle Konfiguration umständlich wäre. Sie bieten mehr Flexibilität als statische Routen, erfordern aber auch mehr Ressourcen und Bandbreite.

## Welche Routing Protokolle kennen Sie?

- RIP (Routing Information Protocol): Ein Distanzvektor-Protokoll für Intradomain-Routing
- OSPF (Open Shortest Path First): Ein Link-State-Protokoll für IPv4 und IPv6, bekannt für schnelle Konvergenz und gute Skalierbarkeit.

## Was ist das Internet Protokoll (IP)?

Das Internet Protocol (IP) ist ein fundamentales Netzwerkprotokoll, das die Grundlage für die Datenübertragung im Internet bildet.

### Hauptfunktionen

1. **Adressierung**: Jedes Gerät im Internet erhält eine eindeutige IP-Adresse zur Identifikation. 
2. **Paketierung**: Daten werden in kleine Einheiten, sogenannte Pakete, aufgeteilt. 
3. **Routing**: IP ist verantwortlich für die Weiterleitung von Datenpaketen zwischen Netzwerken, um sie von der Quelle zum Ziel zu transportieren. 
4. **Fragmentierung**: Bei Bedarf werden große Datenpakete in kleinere Einheiten aufgeteilt, um sie über verschiedene Netzwerke zu übertragen. 

> [!note]
IP arbeitet verbindungslos, das heißt, jedes Paket wird unabhängig behandelt und kann unterschiedliche Routen nehmen. Es bildet die Grundlage für andere Protokolle wie TCP, die für die Zuverlässigkeit der Übertragung sorgen. Die derzeit am weitesten verbreitete Version ist IPv4, wobei IPv6 zunehmend an Bedeutung gewinnt, da es einen größeren Adressraum bietet

## Erklären Sie den Begriff „RTT“ (Round Trip Time)?

RTT (Round Trip Time) ist die Zeit in Millisekunden, die ein Datenpaket benötigt, um von einem Startpunkt zu einem Ziel und wieder zurück zum Ausgangspunkt zu gelangen. Diese Messgröße ist wichtig für die Beurteilung der Leistung und Effizienz von Netzwerkverbindungen. 

### Hauptmerkmale der RTT

- Misst die Gesamtlatenz einer Netzwerkanfrage
- Umfasst Übertragungszeit, Ausbreitungsverzögerung und Verarbeitungszeit
- Wird oft mit dem "Ping"-Befehl gemessen
- Beeinflusst direkt die Reaktionsfähigkeit von Netzwerkanwendungen

### Faktoren, die die RTT beeinflussen

- Physische Entfernung zwischen Quelle und Ziel
- Netzwerkinfrastruktur und Routing
- Netzwerkverkehr und Überlastung
- Art der Verbindung (z.B. Kupferkabel, Glasfaser, drahtlos)

> [!note]
Eine niedrige RTT ist entscheidend für eine gute Benutzererfahrung, da sie schnellere Ladezeiten und reaktionsschnellere Dienste ermöglicht. Die Optimierung der RTT ist ein Hauptziel von Content Delivery Networks (CDNs) und anderen Netzwerkoptimierungstechniken