---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/Verkabelung.md
sticker: lucide//book-open-check
---
## **Welche Standardgröße wird meistens für Netzwerkschränke verwendet?**

Die am häufigsten verwendete Standardgröße für Netzwerkschränke ist das 19-Zoll-Format. Dieses Format bezieht sich auf die Breite der Montageschienen im Inneren des Schranks und entspricht 48,26 cm.

### Typische Abmessungen für 19-Zoll-Netzwerkschränke

**Breite**
600 mm oder 800 mm

**Tiefe**
600 mm, 800 mm, 1000 mm oder 1200 mm

**Höhe**
Wird in Höheneinheiten (HE) angegeben, wobei 1 HE = 44,45 mm entspricht. Ein häufig verwendeter Standard ist 42 HE, was einer Höhe von ca. 2 m entspricht.

> [!NOTE]
Diese Standardisierung ermöglicht eine hohe Kompatibilität zwischen verschiedenen Herstellern und erleichtert die Organisation und den Einbau von Netzwerkkomponenten

## **Welche Netzwerktopologien kennen Sie?**

Es gibt verschiedene **Netzwerktopologien**, die die Struktur und Verbindung der Geräte in einem Netzwerk beschreiben. Hier sind die wichtigsten:

### 1. Bus-Topologie

**Eigenschaften**

- Alle Geräte sind über ein gemeinsames Kabel (den "Bus") verbunden.
- Daten werden in beide Richtungen gesendet.

**Vorteile**

- Einfacher Aufbau, geringe Kosten
- Weniger Kabelaufwand

**Nachteile**

- Ein Kabelausfall legt das gesamte Netzwerk lahm
- Hohe Kollisionen bei vielen Geräten

**Beispiel**: Ältere Ethernet-Netzwerke (10BASE2, 10BASE5)

### 2. Stern-Topologie

**Eigenschaften**

- Alle Geräte sind mit einem zentralen Knoten (z. B. Switch) verbunden.

**Vorteile**

- Hohe Ausfallsicherheit (nur ein Gerät fällt aus, nicht das gesamte Netzwerk)
- Gute Performance, da keine Datenkollisionen entstehen

**Nachteile**

- Zentrale Komponente ist ein **Single Point of Failure**
- Höherer Kabelaufwand

**Beispiel**: Ethernet-Netzwerke mit Switch

### 3. Ring-Topologie

**Eigenschaften**

- Geräte sind in einem geschlossenen Ring verbunden, Daten bewegen sich in eine Richtung.

**Vorteile**

- Keine Kollisionen, da der Datenfluss geregelt ist
- Vorhersehbare Datenübertragung

**Nachteile**

- Ein defektes Gerät oder Kabel kann das ganze Netzwerk unterbrechen
- Aufwendige Fehlerbehebung

**Beispiel**: Token Ring (veraltet)

### 4. Mesh-Topologie

**Eigenschaften**

- Jeder Knoten ist mit mehreren anderen Knoten verbunden (vollständig oder teilweise).

**Vorteile**

- Sehr hohe Ausfallsicherheit (Redundanz)
- Sehr gute Performance

**Nachteile**

- Hohe Kosten durch viele Kabel/Verbindungen
- Komplexe Konfiguration

**Beispiel**: WAN-Netzwerke, WLAN-Mesh-Netzwerke

### 5. Baum-Topologie (Hierarchisch)

**Eigenschaften**

- Kombination aus Stern- und Bus-Topologie (hierarchische Struktur mit mehreren Ebenen).

**Vorteile**

- Skalierbar und gut organisierbar
- Einfache Erweiterung möglich

**Nachteile**

- Höhere Komplexität
- Fällt eine zentrale Verbindung aus, können ganze Segmente betroffen sein

**Beispiel**: Große Unternehmensnetzwerke

### 6. Hybrid-Topologie

**Eigenschaften**

- Kombination aus verschiedenen Topologien (z. B. Stern-Bus oder Stern-Ring).

**Vorteile**

- Flexibel anpassbar
- Kann die Vorteile mehrerer Topologien kombinieren

**Nachteile**

- Komplizierte Einrichtung
- Hoher Verwaltungsaufwand

 **Beispiel**: Moderne Rechenzentren

### Fazit – Welche ist die beste?

- **Kleine Netzwerke → Stern** (einfach, zuverlässig)
- **Große, ausfallsichere Netzwerke → Mesh oder Hybrid**
- **Einfache, kostengünstige Netze → Bus oder Ring (heute selten)**

 **Merktipp:**

- **Bus** = Eine Datenstraße
- **Stern** = Alle zum Mittelpunkt
- **Ring** = Eine Kreisstraße
- **Mesh** = Jeder mit jedem
- **Baum** = Hierarchie mit Ästen

## **Erklären Sie den Begriff TP-Kabel.**

TP-Kabel, auch als Twisted-Pair-Kabel bezeichnet, sind Netzwerkkabel, die aus paarweise verdrillten Kupferadern bestehen. Die wichtigsten Merkmale von TP-Kabeln sind:

### Aufbau
Mehrere Paare isolierter Kupferdrähte, die miteinander verdrillt sind.

### Schutz
Die Verdrillung bietet Schutz gegen elektromagnetische Störungen.

### Kategorien
Es gibt verschiedene Kategorien (Cat 1 bis Cat 8) mit unterschiedlichen Übertragungseigenschaften.

### Abschirmung
TP-Kabel können ungeschirmt (UTP) oder geschirmt (STP, FTP) sein.

### Anwendungen
Weit verbreitet in Computernetzwerken, Ethernet-Verbindungen und Telefonleitungen.

> [!NOTE]
TP-Kabel sind aufgrund ihrer Flexibilität, einfachen Installation und Kosteneffizienz die am häufigsten verwendeten Kabel in modernen Netzwerkinfrastrukturen

## **Wozu werden einzelne Adernpaare verdrillt?**

### Zweck der Verdrillung 

- Reduzierung elektromagnetischer Störungen: Die Verdrillung verringert die Anfälligkeit für externe elektromagnetische Interferenzen. 
- Minimierung des Übersprechens: Sie reduziert das Übersprechen zwischen benachbarten Adernpaaren innerhalb des Kabels. 
- Gleichtaktauslöschung: Störungen wirken sich theoretisch auf beide Drähte des Paares gleich aus und heben sich dadurch gegenseitig auf. 
- Verbesserung der Datenübertragung: Durch die Reduzierung von Störungen ermöglicht die Verdrillung eine schnellere und zuverlässigere Übertragung von Daten. 
- Symmetrische Signalübertragung: Die Verdrillung unterstützt die symmetrische Übertragung von Signalen, was die Störanfälligkeit weiter reduziert.

> [!note]
Diese Eigenschaften machen Twisted-Pair-Kabel zu einer effektiven Lösung für die Netzwerkkommunikation, insbesondere in Umgebungen mit potenziellen elektromagnetischen Störquellen.

**Welche unterschiedlichen TP-Kabel kennen Sie?**
 
### TP-Kabel & Specs 
  
**UTP (Unshielded Twisted Pair)**
Kabel ohne zusätzliche Abschirmung. 

**F/UTP (Foiled Unshielded Twisted Pair)** 
Kabel mit einer Aluminiumfolie als Gesamtabschirmung. 

**S/UTP (Screened Unshielded Twisted Pair)** 
Kabel mit einem Kupfergeflecht als Gesamtabschirmung 

**S/FTP (Screened Foiled Twisted Pair)** 
Kabel mit Gesamtabschirmung aus Kupfergeflecht und zusätzlicher Folienabschirmung der einzelnen Adernpaare. 

**S/STP (Screened Shielded Twisted Pair)** 
Kabel mit Gesamtabschirmung und zusätzlicher Abschirmung der einzelnen Adernpaare.

> [!NOTE]
Zudem werden TP-Kabel in verschiedene Kategorien (Cat 1 bis Cat 8) eingeteilt, die sich in ihrer Leistungsfähigkeit und maximalen Übertragungsfrequenz unterscheiden

## **Wie viel beträgt die maximale Kabellänge von Kupfer-Netzwerkkabeln?**

Die maximale Kabellänge von Kupfer-Netzwerkkabeln beträgt in der Regel 100 Meter. 
Dies gilt für die gängigen Ethernet-Standards wie Cat5e, Cat6 und Cat6a. 
Diese Begrenzung auf 100 Meter pro Netzwerksegment ist wichtig, um eine optimale Signalqualität und Übertragungsgeschwindigkeit zu gewährleisten.

## **Wie kann ein Cat7 Kabel verlängert werden?**

### Verbindungsmodul
Spezielle Verbindungsmodule für Cat7-Leitungen können verwendet werden, um zwei Kabelenden zu verbinden. 

### Koppler
Ein einfacher Ethernet-Koppler verbindet zwei Cat7-Kabel miteinander. 

### Netzwerk-Switch
Durch Platzierung eines Switches zwischen zwei Kabeln kann die Gesamtreichweite vergrößert werden. 

### Medienkonverter
Diese wandeln das Ethernet-Signal in ein Glasfasersignal um, was deutlich größere Distanzen ermöglicht. 

### Ethernet-Extender
Diese Geräte nutzen DSL-Technologie, um Ethernet-Signale über längere Strecken zu übertragen. 

### Netzwerkdosen
Installation von Netzwerkdosen an beiden Enden der zu verlängernden Strecke.

> [!NOTE]
Bei der Verlängerung sollte beachtet werden, dass die Gesamtlänge von 100 Metern pro Segment nicht überschritten wird, um Signalverluste zu vermeiden. Für Distanzen über 100 Meter sind spezielle Lösungen wie Medienkonverter oder Ethernet-Extender erforderlich.

## **Nennen Sie den Unterschied von Cat5e und Cat7.**

### Übertragungsgeschwindigkeit

**Cat5e**
bis zu 1 Gbit/s

**Cat7**
bis zu 10 Gbit/s (bei 100 m), 40 Gbit/s (bei 50 m) oder sogar 100 Gbit/s (bei 15 m)

### Frequenzbereich

**Cat5e**
bis zu 100 MHz

**Cat7**
bis zu 600 MHz (Cat7a sogar bis zu 1000 MHz)

### Abschirmung

**Cat5e**
in der Regel ungeschirmt (UTP)

**Cat7**
vollständig geschirmt (S/FTP oder F/FTP) mit 4 separat abgeschirmten Adernpaaren

### Anwendungsbereich

**Cat5e**
häufig in Privatanwendungen und älteren Installationen

**Cat7**
professionelle Umgebungen, Rechenzentren, Neubauten mit hochwertiger Netzwerkverkabelung

### Steckertypen

**Cat5e**
RJ45

**Cat7**
RJ45 oder GG45 (für volle Bandbreitennutzung)

> [!NOTE]
Cat7 bietet insgesamt eine deutlich höhere Leistung und besseren Schutz gegen elektromagnetische Störungen, ist aber auch teurer und weniger flexibel als Cat5e.

## **Erklären Sie den Begriff „RJ45“.**

Der Begriff RJ45 steht für **„Registered Jack 45“** und bezeichnet eine standardisierte Steckverbindung, die hauptsächlich in Netzwerken verwendet wird. RJ45-Stecker sind die am häufigsten genutzten Anschlüsse für Ethernet-Kabel und ermöglichen die Verbindung von Geräten wie Computern, Routern und Switches. 

### Merkmale und Funktionen

**Aufbau**
RJ45-Stecker haben 8 Kontakte (8P8C – 8 Positionen, 8 Kontakte), die mit den Adern eines Twisted-Pair-Kabels verbunden sind.

**Verwendung**
Sie dienen der Datenübertragung in lokalen Netzwerken (LAN) und unterstützen hohe Übertragungsraten, z. B. Gigabit-Ethernet.

**Standards**
Die Verdrahtung erfolgt nach den Standards T568A oder T568B.

**Anwendungsbereiche**
Heimnetzwerke, Unternehmensnetzwerke, Telekommunikation.

> [!NOTE]
RJ45-Stecker sind universell einsetzbar, einfach zu installieren und bilden das Rückgrat kabelgebundener Netzwerke.

## **Erklären Sie die Vorteile von Patchpanel und Patchdosen.**

Patchpanels und Patchdosen bieten mehrere Vorteile für die Netzwerkinfrastruktur:

### Vorteile von Patchpanels

**Organisation und Effizienz**
Patchpanels halten Kabel ordentlich und organisiert, was Unordnung vermeidet und die Effizienz steigert. 

**Skalierbarkeit**
Sie ermöglichen einfaches Hinzufügen, Löschen oder Ändern von Netzwerkkonfigurationen. 

**Reduzierte Ausfallzeiten**
Fehlerbehebung und Wartung werden vereinfacht, was die Netzwerk-Ausfallzeit reduziert. 

**Schutz**
Patchpanels schützen empfindliche Anschlüsse von Netzwerkkabeln vor physischer Beschädigung. 

**Flexibilität**
Sie ermöglichen das Anschließen von Kabeln von jedem Gerät an jeden Port, ohne das gesamte Netzwerk neu verkabeln zu müssen. 

**Zentrale Verwaltung**
Patchpanels bieten einen zentralen Ort für alle Kabelanschlüsse, was Netzwerkänderungen vereinfacht.

### Vorteile von Patchdosen

**Strukturierte Verkabelung**
Patchdosen dienen als Endpunkte der Netzwerkverkabelung und ermöglichen eine strukturierte, fest verkabelte Ethernet-Netzwerkinfrastruktur. 

**Flexibilität**
Sie erlauben das einfache Anschließen und Umstecken von Geräten an verschiedenen Orten im Netzwerk. 

**Störungsfreie Verbindung**
Patchdosen ermöglichen eine zuverlässige und störungsfreie Verbindung zwischen Geräten. 

**Skalierbarkeit**
Durch die Verwendung von Patchdosen kann das Netzwerk einfach erweitert oder umstrukturiert werden.

> [!note]
Sowohl Patchpanels als auch Patchdosen tragen zu einer effizienten, flexiblen und gut organisierten Netzwerkinfrastruktur bei, die einfach zu warten und zu erweitern ist.

## **Erklären Sie den Aufbau eines Koaxialkabels.**

Ein Koaxialkabel besteht aus mehreren konzentrischen Schichten, die für Signalübertragung und Abschirmung sorgen.

### Innenleiter
Kupferdraht oder -litze, leitet das Signal.

### Dielektrikum
Isolierende Schicht aus Kunststoff, trennt Innenleiter und Außenleiter.

### Außenleiter
Geflecht oder Folie aus Metall, dient als Abschirmung gegen elektromagnetische Störungen und Rückleiter.

### Außenmantel
Schutzhülle aus Kunststoff, schützt das Kabel vor mechanischen Einflüssen.

> [!NOTE]
Koaxialkabel werden häufig für TV-, Breitband- und Hochfrequenzanwendungen verwendet.

## **Erklären Sie den Aufbau eines LWL-Kabels.**

Ein LWL-Kabel (Lichtwellenleiterkabel) besteht aus mehreren Schichten, die speziell für die Übertragung von Lichtsignalen ausgelegt sind.

### Kern (Core)
Dünner Glas- oder Kunststofffaserbereich, durch den das Lichtsignal transportiert wird.

### Mantel (Cladding)
Umgibt den Kern, hat einen niedrigeren Brechungsindex, um das Licht durch Totalreflexion im Kern zu halten.

### Primärbeschichtung
Schützende Kunststoffschicht direkt um den Mantel, schützt vor mechanischen Schäden.

### Sekundärmantel
Weitere Schutzschicht, oft aus Kunststoff, um Stabilität und zusätzlichen Schutz zu bieten.

### Stärkungselemente
Glasfasern, Aramidfasern (z. B. Kevlar) oder Stahldrähte, die Zugentlastung und Stabilität bieten.

### Außenmantel
Robuste Hülle aus Kunststoff, schützt das Kabel vor Umwelteinflüssen wie Feuchtigkeit, Abrieb und UV-Strahlung.

> [!NOTE]
LWL-Kabel werden für Hochgeschwindigkeitsdatenübertragungen und in störanfälligen Umgebungen eingesetzt.

## **Welche Arten von LWL-Kabeln kennen Sie?**

Es gibt zwei Hauptarten von LWL-Kabeln, die sich durch ihre Übertragungseigenschaften unterscheiden:

### Singlemode-Faser (SMF)

- Sehr dünner Kern (~9 µm Durchmesser).
- Überträgt Licht mit nur einem Modus (geringe Streuung).
- Geeignet für weite Entfernungen und hohe Datenraten (z. B. in Fernverbindungen, Backbone-Netzen).

### Multimode-Faser (MMF)

- Größerer Kern (~50 oder 62,5 µm Durchmesser).
- Überträgt mehrere Lichtmoden gleichzeitig (mehr Streuung).
- Geeignet für kürzere Entfernungen (z. B. in LANs und Gebäuden).

## **Wozu wird ein LWL-Kabel mit einem Kerndurchmesser von 125/50μ verwendet?**

Ein LWL-Kabel mit einem Kerndurchmesser von 125/50 µm ist ein Multimode-Kabel und wird für folgende Anwendungen genutzt:

- Kurzstreckenverbindungen (z. B. innerhalb von Gebäuden oder Rechenzentren).
- LANs und SANs (lokale und Speicher-Netzwerke).
- Datenübertragung mit moderaten Geschwindigkeiten (typisch bis zu 10 Gbit/s, abhängig von der Entfernung).

> [!note]
Der Kern (50 µm) führt das Lichtsignal, während der Mantel (125 µm) die Lichtführung durch Totalreflexion unterstützt.

## **Wozu wird ein LWL-Kabel mit einem Kerndurchmesser von 125/3 bis 9 μ verwendet?**

Ein LWL-Kabel mit einem Kerndurchmesser von 125/3 bis 9 µm ist ein Singlemode-Kabel.

### Anwendungsbereich

- Langstreckenverbindungen (z. B. zwischen Städten, Ländern oder in Backbone-Netzwerken).
- Hohe Datenübertragungsraten (10 Gbit/s bis 400 Gbit/s oder mehr).
- Telekommunikationsnetze und Internet-Backbones, wo geringe Signalverluste und Dispersion entscheidend sind.

> [!note]
Der kleine Kern (3 bis 9 µm) minimiert Lichtstreuung und ermöglicht eine präzise Signalübertragung über große Distanzen.

## **Was für eine Wellenlänge wird üblicherweise bei Singlemode-Kabeln verwendet?**

### Singlemode Wellenlängen

- 1310 nm: Für Kurz- bis Mittelstreckenverbindungen.
- 1550 nm: Für Langstreckenverbindungen, da hier die Dämpfung in der Faser am geringsten ist.
- 1625 nm: Für spezielle Anwendungen wie Überwachung und zusätzliche Kanäle in WDM-Systemen.

> [!note]
Diese Wellenlängen liegen im Infrarotbereich und sind optimal für die Übertragung in Glasfasern.

## **Was für eine Wellenlänge wird üblicherweise bei Multimode-Kabeln verwendet?**

### Multimode Wellenlängen

- 850 nm: Standardwellenlänge für Kurzstrecken und kostengünstige Transceiver.
- 1300 nm: Für längere Strecken innerhalb von Multimode-Anwendungen, mit geringerer Dämpfung als 850 nm.

>[!note]
Diese Wellenlängen sind ideal für typische Multimode-Anwendungen in lokalen Netzwerken und Rechenzentren.

## **Was verstehen Sie unter der Bezeichnung z.B. OM3, OS1, uä.**

### OM und OS – Glasfaserkabel-Kategorien

Die Bezeichnungen OM und OS kennzeichnen Multimode- bzw. Singlemode-Glasfaserkabel mit spezifischen Leistungsmerkmalen.

#### OM (Optical Multimode) – Für kürzere Distanzen

- **OM1:** 1 Gbit/s, 62,5 µm-Kern, bis 300 m (850 nm)
- **OM2:** 1 Gbit/s, 50 µm-Kern, bis 550 m (850 nm)
- **OM3:** Optimiert für 10 Gbit/s, bis 300 m (850 nm)
- **OM4:** 10 Gbit/s bis 550 m, 100 Gbit/s bis 150 m

#### OS (Optical Singlemode) – Für große Distanzen

- **OS1:** Bis 10 km, verlustarm
- **OS2:** Für >10 km, minimaler Signalverlust

## **Wie hoch ist die maximale Übertragungsdistanz bei Singlemode-Kabeln?**

Die maximale Übertragungsdistanz bei Singlemode-Glasfaserkabeln hängt von Faktoren wie der verwendeten Technik, dem Wellenlängenbereich und der Signalverstärkung ab. 
### Ohne Verstärker
Bis zu 10 km (OS1) und 40 km (OS2).

### Mit Verstärkern (z. B. EDFA) oder DWDM-Technologie
Über 80 km und bis zu Hunderten von Kilometern.

> [!note]
Singlemode-Kabel sind daher ideal für Langstrecken- und Hochgeschwindigkeitsnetzwerke.

## **Wie hoch ist die maximale Übertragungsdistanz bei Multimode-Kabeln?**

Die maximale Übertragungsdistanz bei Multimode-Glasfaserkabeln hängt von der Kabelkategorie (OM1–OM5), dem Wellenlängenbereich und der Übertragungsgeschwindigkeit ab.

### OM1
Bis zu 300 m bei 1 Gbit/s.

### OM2
Bis zu 550 m bei 1 Gbit/s.

### OM3
Bis zu 300 m bei 10 Gbit/s, 100 m bei 40/100 Gbit/s.

### OM4
Bis zu 550 m bei 10 Gbit/s, 150 m bei 40/100 Gbit/s.

### OM5
Ähnlich OM4, unterstützt aber breitere Wellenlängenbereiche (SWDM).

> [!note]
Multimode-Kabel eignen sich für kürzere Distanzen innerhalb von Gebäuden oder Rechenzentren.

## **Welche Vorteile bzw Nachteile bieten LWL-Kabel?**

### Vorteile von LWL-Kabeln

- Hohe Übertragungsgeschwindigkeit und Bandbreite.
- Geringe Signalverluste, ideal für große Entfernungen.
- Immunität gegen elektromagnetische Störungen.
- Keine elektrische Leitfähigkeit, daher sicher gegen Blitzschlag.
- Leicht und dünn, einfach zu verlegen.

### Nachteile von LWL-Kabeln

- Höhere Kosten für Kabel und Geräte (Transceiver).
- Empfindlich gegenüber Biegungen und mechanischen Belastungen.
- Aufwändigere Installation und Reparatur (Spleißen).
- Spezialisierte Fachkenntnisse für Wartung erforderlich.

## **Wo werden Lichtwellenleiter eingesetzt?**

Lichtwellenleiter (LWL) werden in verschiedenen Bereichen eingesetzt, wo hohe Bandbreiten und zuverlässige Datenübertragung über lange Distanzen erforderlich sind.

### Telekommunikation
Backbone-Netzwerke für Internet, Telefonie und TV.

### Rechenzentren
Verbindung von Servern und Speichern mit hoher Geschwindigkeit.

### Unterseekabel
Internationale Datenverbindungen über Ozeane.

### Industrie
Automatisierung, Steuerungssysteme und sichere Datenübertragung.

### Medizin
Endoskope und Laser für präzise Anwendungen.

### Militär und Sicherheit
Abhörsichere und störungsfreie Kommunikation.

### Verkehr
Vernetzung von Signalanlagen und Überwachungssystemen.

### Energie
Übertragung von Daten in Kraftwerken oder Stromnetzen.

## **Welche Typen von LWL-Steckverbindern kennen Sie?**

### Bekannte Typen von LWL-Steckverbindern

**LC (Lucent Connector)**
Kompakt, für hohe Dichte, häufig in Rechenzentren.

**SC (Subscriber Connector)**
Quadratisch, leicht zu handhaben, oft in Netzwerken.

**ST (Straight Tip)**
Rund, Bajonettverschluss, für ältere Installationen.

**FC (Ferrule Connector)**
Rund, verschraubt, für hohe Stabilität.

**MPO/MTP (Multi-Fiber Push-On/Pull-Off)**
Mehrfaser-Steckverbinder, für Parallelübertragungen.

**E2000**
Mit selbstschließendem Schutzdeckel, für hohe Sicherheitsanforderungen.

**DIN-Stecker**
Für industrielle Anwendungen.

> [!note]
Diese Steckverbinder werden je nach Anforderungen an Dichte, Stabilität und Anwendung ausgewählt.

## **Was versteht man unter dem Begriff „Dark-Fibre“?**

Der Begriff Dark Fibre bezeichnet ungenutzte oder unbeleuchtete Glasfaserkabel, die zwar verlegt, aber aktuell nicht aktiv in Betrieb sind.

### Verwendung und Vorteile

- Unternehmen oder Anbieter können Dark Fibre mieten oder kaufen und sie mit eigener Hardware betreiben, um volle Kontrolle über Bandbreite und Sicherheit zu haben.
- Sie wird oft für maßgeschneiderte Netzwerklösungen oder langfristige Kapazitätsreserven genutzt.

> [!note]
Dark Fibre ermöglicht hohe Flexibilität, erfordert jedoch Investitionen in aktive Netzkomponenten, um sie nutzbar zu machen.

## **Erklären Sie den Begriff „Dispersion“ im Zusammenhang mit Lichtwellenleitern.**

Dispersion in Lichtwellenleitern beschreibt die Aufspaltung eines Lichtsignals in unterschiedliche Komponenten, was zu einer Verbreiterung des Signals über die Zeit führt. Dies kann die Signalqualität und Übertragungsgeschwindigkeit beeinträchtigen. 

### Hauptarten

**Modendispersion**
Tritt in Multimode-Fasern auf, da verschiedene Lichtmoden unterschiedliche Wege und somit unterschiedliche Laufzeiten haben.

**Chromatische Dispersion**
Entsteht durch unterschiedliche Brechungsindizes für verschiedene Wellenlängen des Lichts, was die Laufzeiten verändert.

**Polarisationsmodendispersion (PMD)**
Tritt in Singlemode-Fasern auf, wenn Polarisationen unterschiedlich schnell durch die Faser laufen.

>[!note]
Dispersion wird durch spezielle Fasertypen (z. B. Dispersion-Shifted Fibre) und optische Komponenten kompensiert, um die Übertragungsleistung zu optimieren.
