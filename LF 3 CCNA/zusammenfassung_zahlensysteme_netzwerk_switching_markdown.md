# Zusammenfassung – Zahlensysteme, Netzwerk-Grundlagen und Ethernet Switching

_Basierend auf den Modulen M05, M06 und M07._

---

# 1. Zahlensysteme für IT-Einsteiger

## 1.1 Warum Zahlensysteme in der IT wichtig sind

Computer arbeiten intern ausschließlich mit elektrischen Zuständen. Diese Zustände werden vereinfacht als:

- Strom vorhanden = 1
- Strom nicht vorhanden = 0

interpretiert.

Daraus entsteht das Binärsystem, welches die Grundlage sämtlicher digitaler Technik bildet.

Zahlensysteme werden in der IT benötigt für:

- Speicheradressierung
- Netzwerkkommunikation
- Maschinenbefehle
- Darstellung von Farben
- Verarbeitung von Daten
- Hardware-nahe Programmierung
- Subnetting und IP-Adressierung

---

# 1.2 Überblick über wichtige Zahlensysteme

| Zahlensystem | Basis | Verwendete Zeichen |
|---|---|---|
| Dezimal | 10 | 0–9 |
| Binär | 2 | 0–1 |
| Oktal | 8 | 0–7 |
| Hexadezimal | 16 | 0–9, A–F |

---

# 1.3 Stellenwertsystem

Jede Stelle einer Zahl besitzt abhängig von ihrer Position einen bestimmten Wert.

## Beispiel Dezimal

Die Zahl:

```text
583
```

bedeutet:

```text
5 × 10² = 500
8 × 10¹ = 80
3 × 10⁰ = 3
```

Gesamt:

```text
500 + 80 + 3 = 583
```

---

# 1.4 Das Binärsystem

Im Binärsystem existieren nur zwei Zustände:

- 0
- 1

Jede Stelle repräsentiert eine Zweierpotenz.

| Bitposition | Wert |
|---|---|
| 7 | 128 |
| 6 | 64 |
| 5 | 32 |
| 4 | 16 |
| 3 | 8 |
| 2 | 4 |
| 1 | 2 |
| 0 | 1 |

## Beispiel

```text
10110110₂
```

Berechnung:

```text
1×128 = 128
0×64 = 0
1×32 = 32
1×16 = 16
0×8 = 0
1×4 = 4
1×2 = 2
0×1 = 0
```

Ergebnis:

```text
182₁₀
```

---

# 1.5 Bit, Byte und Speichergrößen

## Bit

Kleinste Informationseinheit:

```text
0 oder 1
```

## Byte

```text
1 Byte = 8 Bit
```

## Speichergrößen

| Einheit | Größe |
|---|---|
| Kilobyte (KB) | 1024 Byte |
| Megabyte (MB) | 1024 KB |
| Gigabyte (GB) | 1024 MB |
| Terabyte (TB) | 1024 GB |

---

# 1.6 Umrechnung Dezimal → Binär

Methode:

1. Zahl durch 2 teilen
2. Rest notieren
3. Ergebnis erneut durch 2 teilen
4. Wiederholen bis Ergebnis 0
5. Reste von unten nach oben lesen

## Beispiel: 25

```text
25 : 2 = 12 Rest 1
12 : 2 = 6 Rest 0
6 : 2 = 3 Rest 0
3 : 2 = 1 Rest 1
1 : 2 = 0 Rest 1
```

Ergebnis:

```text
11001₂
```

---

# 1.7 Umrechnung Binär → Dezimal

Jede gesetzte Stelle wird addiert.

## Beispiel

```text
11001₂
```

```text
1×16 = 16
1×8 = 8
0×4 = 0
0×2 = 0
1×1 = 1
```

Ergebnis:

```text
25₁₀
```

---

# 1.8 Das Hexadezimalsystem

Das Hexadezimalsystem verwendet 16 Zeichen:

```text
0–9 und A–F
```

| Hex | Dezimal |
|---|---|
| A | 10 |
| B | 11 |
| C | 12 |
| D | 13 |
| E | 14 |
| F | 15 |

Hexadezimal wird genutzt, weil lange Binärzahlen kompakter dargestellt werden können.

---

# 1.9 Zusammenhang Binär ↔ Hexadezimal

4 Bit entsprechen exakt einer Hex-Ziffer.

| Binär | Hex |
|---|---|
| 0000 | 0 |
| 0001 | 1 |
| 0010 | 2 |
| 0011 | 3 |
| 0100 | 4 |
| 0101 | 5 |
| 0110 | 6 |
| 0111 | 7 |
| 1000 | 8 |
| 1001 | 9 |
| 1010 | A |
| 1011 | B |
| 1100 | C |
| 1101 | D |
| 1110 | E |
| 1111 | F |

---

# 1.10 Umrechnung Binär → Hex

Bits in Vierergruppen aufteilen.

## Beispiel

```text
110101101011
```

Aufteilung:

```text
1101 0110 1011
```

Umrechnung:

```text
1101 = D
0110 = 6
1011 = B
```

Ergebnis:

```text
D6B₁₆
```

---

# 1.11 ASCII und Zeichencodierung

Computer speichern Zeichen intern ebenfalls als Zahlen.

## ASCII

ASCII verwendet 7 Bit.

Beispiele:

| Zeichen | ASCII |
|---|---|
| A | 65 |
| B | 66 |
| a | 97 |

---

# 1.12 Unicode

ASCII reicht für moderne Sprachen nicht aus.

Unicode ermöglicht:

- Sonderzeichen
- Umlaute
- Emojis
- internationale Schriftsysteme

Wichtige Formate:

- UTF-8
- UTF-16
- UTF-32

UTF-8 ist heute Standard im Web.

---

# 1.13 Logische Operationen

Digitale Schaltungen basieren auf Boolescher Algebra.

## AND

Nur wahr, wenn beide Eingänge wahr sind.

| A | B | Ergebnis |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

## OR

Mindestens ein Eingang muss wahr sein.

## NOT

Negiert den Eingang.

---

# 1.14 Bedeutung für die Fachinformatik

Zahlensysteme sind Grundlage für:

- Netzwerktechnik
- Speicheradressierung
- Programmierung
- Datenübertragung
- Fehlersuche
- Sicherheitstechnik
- Embedded Systems
- Betriebssysteme

Insbesondere Subnetting und MAC-/IP-Adressierung basieren direkt auf Binärdarstellung.

---

# 2. Netzwerk-Grundlagen

## 2.1 Was ist ein Netzwerk?

Ein Netzwerk verbindet mehrere Geräte zur gemeinsamen Nutzung von:

- Daten
- Diensten
- Druckern
- Internetzugängen
- Ressourcen

Geräte in Netzwerken heißen:

- Hosts
- Clients
- Endgeräte

---

# 2.2 Ziele von Netzwerken

- Datenaustausch
- Kommunikation
- Zentrale Verwaltung
- Ressourcenteilung
- Ausfallsicherheit
- Skalierbarkeit

---

# 2.3 Netzwerkarten

| Typ | Bedeutung |
|---|---|
| PAN | Personal Area Network |
| LAN | Local Area Network |
| WLAN | Wireless LAN |
| MAN | Metropolitan Area Network |
| WAN | Wide Area Network |
| GAN | Global Area Network |

---

# 2.4 Netzwerkkomponenten

## Switch

Verbindet Geräte innerhalb eines LANs.

Arbeitet auf:

- OSI-Schicht 2

Verwendet:

- MAC-Adressen

---

## Router

Verbindet verschiedene Netzwerke.

Arbeitet auf:

- OSI-Schicht 3

Verwendet:

- IP-Adressen

---

## Access Point

Stellt drahtlose Verbindungen bereit.

---

## Modem

Wandelt digitale und analoge Signale um.

---

# 2.5 Netzwerk-Topologien

## Bus

Alle Geräte teilen sich eine Leitung.

Nachteil:

- Kollisionen
- Fehleranfällig

---

## Stern

Alle Geräte sind mit zentralem Switch verbunden.

Heute Standard.

Vorteile:

- Gute Erweiterbarkeit
- Fehler leicht lokalisierbar

---

## Ring

Geräte bilden geschlossenen Kreis.

---

## Mesh

Viele direkte Verbindungen.

Hohe Ausfallsicherheit.

---

# 2.6 Das OSI-Modell

Das OSI-Modell beschreibt Netzwerkkommunikation in 7 Schichten.

| Schicht | Name | Aufgabe |
|---|---|---|
| 7 | Anwendung | Benutzernahe Dienste |
| 6 | Darstellung | Kodierung, Verschlüsselung |
| 5 | Sitzung | Sitzungssteuerung |
| 4 | Transport | Zuverlässige Übertragung |
| 3 | Vermittlung | Routing |
| 2 | Sicherung | Frames, MAC-Adressen |
| 1 | Bitübertragung | Elektrische Signale |

---

# 2.7 TCP/IP-Modell

Praxisorientiertes Modell des Internets.

| TCP/IP | Entspricht OSI |
|---|---|
| Anwendung | 5–7 |
| Transport | 4 |
| Internet | 3 |
| Netzzugang | 1–2 |

---

# 2.8 Datenkapselung

Beim Senden werden Daten schichtweise verpackt.

| Schicht | Dateneinheit |
|---|---|
| Anwendung | Daten |
| Transport | Segment |
| Vermittlung | Paket |
| Sicherung | Frame |
| Bitübertragung | Bits |

---

# 2.9 MAC-Adresse

Eindeutige Hardwareadresse eines Netzwerkadapters.

Eigenschaften:

- 48 Bit
- Hexadezimale Darstellung
- Weltweit eindeutig

## Aufbau

| Teil | Bedeutung |
|---|---|
| OUI | Herstellerkennung |
| NIC | Gerätekennung |

Beispiel:

```text
00:1A:2B:4C:5D:6E
```

---

# 2.10 IPv4-Adressen

IPv4 verwendet:

```text
32 Bit
```

Darstellung:

```text
192.168.0.1
```

Vier Oktette:

```text
8 Bit + 8 Bit + 8 Bit + 8 Bit
```

---

# 2.11 Öffentliche und private IP-Adressen

## Private Bereiche

| Bereich |
|---|
| 10.0.0.0/8 |
| 172.16.0.0 – 172.31.255.255 |
| 192.168.0.0/16 |

Nicht direkt im Internet routbar.

---

# 2.12 Subnetzmaske

Trennt:

- Netzwerkanteil
- Hostanteil

## Beispiel

```text
255.255.255.0
```

entspricht:

```text
/24
```

---

# 2.13 Standardgateway

Router-Adresse zum Verlassen des eigenen Netzwerks.

Ohne Gateway:

- nur Kommunikation im lokalen Netz

---

# 2.14 DNS

Domain Name System.

Übersetzt:

```text
www.example.com
```

in:

```text
IP-Adresse
```

---

# 2.15 DHCP

Dynamic Host Configuration Protocol.

Vergibt automatisch:

- IP-Adresse
- Gateway
- DNS
- Subnetzmaske

---

# 2.16 Wichtige Protokolle

| Protokoll | Zweck |
|---|---|
| HTTP | Webseiten |
| HTTPS | Verschlüsselte Webseiten |
| FTP | Dateiübertragung |
| SSH | Sichere Fernverwaltung |
| DNS | Namensauflösung |
| DHCP | Adressvergabe |
| ICMP | Diagnose |
| TCP | Zuverlässiger Transport |
| UDP | Schneller Transport |

---

# 2.17 TCP und UDP

## TCP

Eigenschaften:

- verbindungsorientiert
- zuverlässig
- Fehlerkontrolle
- Reihenfolge garantiert

Verwendet bei:

- Webseiten
- Dateiübertragung
- E-Mail

---

## UDP

Eigenschaften:

- verbindungslos
- schnell
- keine Garantie

Verwendet bei:

- Streaming
- VoIP
- Online-Spielen

---

# 2.18 Ports

Ports identifizieren Dienste.

| Port | Dienst |
|---|---|
| 20/21 | FTP |
| 22 | SSH |
| 25 | SMTP |
| 53 | DNS |
| 80 | HTTP |
| 443 | HTTPS |

---

# 2.19 ICMP und Ping

ICMP dient Diagnosezwecken.

Bekannte Befehle:

```bash
ping
```

```bash
tracert
```

---

# 2.20 ARP

Address Resolution Protocol.

Übersetzt:

```text
IP-Adresse → MAC-Adresse
```

Innerhalb lokaler Netzwerke.

---

# 2.21 NAT

Network Address Translation.

Router übersetzen:

- private IPs
- öffentliche IPs

Dadurch können mehrere Geräte eine öffentliche Adresse nutzen.

---

# 2.22 IPv6

IPv4-Adressen werden knapp.

IPv6 verwendet:

```text
128 Bit
```

Beispiel:

```text
2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

Vorteile:

- deutlich mehr Adressen
- effizienteres Routing
- bessere Autokonfiguration

---

# 2.23 Netzwerkdiagnose

Wichtige Befehle:

## Windows

```bash
ipconfig
```

```bash
ping
```

```bash
tracert
```

```bash
nslookup
```

---

## Linux

```bash
ifconfig
```

oder:

```bash
ip a
```

---

# 3. Ethernet Switching

## 3.1 Grundlagen von Ethernet

Ethernet ist der Standard für kabelgebundene Netzwerke.

Eigenschaften:

- IEEE 802.3
- Frame-basierte Kommunikation
- MAC-Adressen
- Layer-2-Technologie

---

# 3.2 Aufgaben eines Switches

Switches:

- verbinden Geräte
- leiten Frames weiter
- lernen MAC-Adressen
- reduzieren Kollisionen
- erhöhen Effizienz

---

# 3.3 Unterschiede Hub und Switch

| Hub | Switch |
|---|---|
| Sendet an alle | Sendet gezielt |
| Viele Kollisionen | Kaum Kollisionen |
| Shared Medium | Eigene Kollisionsdomänen |
| Layer 1 | Layer 2 |

---

# 3.4 MAC-Adress-Tabelle

Switches speichern:

- MAC-Adresse
- zugehörigen Port

Dadurch können Frames gezielt weitergeleitet werden.

---

# 3.5 Switching-Prozess

## Schritt 1

Frame trifft ein.

## Schritt 2

Quell-MAC wird gelernt.

## Schritt 3

Ziel-MAC wird gesucht.

## Schritt 4

Frame wird weitergeleitet.

---

# 3.6 Flooding

Ist Ziel unbekannt:

- Switch sendet an alle Ports
- außer Eingangsport

---

# 3.7 Broadcast

Broadcast-Adresse:

```text
FF:FF:FF:FF:FF:FF
```

Alle Geräte erhalten den Frame.

---

# 3.8 Unicast

Frame an genau ein Ziel.

Standardfall moderner Netzwerke.

---

# 3.9 Multicast

Frame an definierte Gruppe.

Verwendung:

- Streaming
- IPTV
- Videokonferenzen

---

# 3.10 Ethernet-Frame

Aufbau eines Ethernet-Frames:

| Bestandteil | Funktion |
|---|---|
| Präambel | Synchronisation |
| Ziel-MAC | Empfänger |
| Quell-MAC | Sender |
| Typ/Länge | Protokolltyp |
| Daten | Nutzdaten |
| FCS | Fehlererkennung |

---

# 3.11 FCS – Frame Check Sequence

Dient Fehlererkennung.

Basierend auf:

- CRC (Cyclic Redundancy Check)

Fehlerhafte Frames werden verworfen.

---

# 3.12 Kollisionsdomänen

## Hub

Alle Geräte teilen eine Kollisionsdomäne.

## Switch

Jeder Port besitzt eigene Kollisionsdomäne.

---

# 3.13 Broadcast-Domänen

Broadcasts werden standardmäßig an alle Ports weitergeleitet.

Router trennen Broadcast-Domänen.

---

# 3.14 Halbduplex und Vollduplex

## Halbduplex

- Senden oder Empfangen
- nicht gleichzeitig

Beispiel:

- Walkie-Talkie

---

## Vollduplex

- gleichzeitiges Senden und Empfangen

Beispiel:

- moderne Ethernet-Verbindungen

---

# 3.15 CSMA/CD

Carrier Sense Multiple Access / Collision Detection.

Wichtig bei alten Shared-Media-Netzen.

Ablauf:

1. Leitung prüfen
2. Senden
3. Kollision erkennen
4. Zufällige Wartezeit
5. Neu senden

Heute wegen Switches weitgehend irrelevant.

---

# 3.16 Auto-Negotiation

Geräte handeln automatisch aus:

- Geschwindigkeit
- Duplex-Modus

---

# 3.17 Ethernet-Geschwindigkeiten

| Standard | Geschwindigkeit |
|---|---|
| Ethernet | 10 Mbit/s |
| Fast Ethernet | 100 Mbit/s |
| Gigabit Ethernet | 1000 Mbit/s |
| 10 Gigabit Ethernet | 10 Gbit/s |

---

# 3.18 Kabeltypen

## Twisted Pair

Standard im LAN.

Kategorien:

| Kategorie | Geschwindigkeit |
|---|---|
| Cat5e | bis 1 Gbit |
| Cat6 | bis 10 Gbit |
| Cat6a | stabilere 10 Gbit |
| Cat7 | höhere Abschirmung |

---

## Glasfaser

Vorteile:

- hohe Geschwindigkeit
- große Reichweite
- störungsarm

---

# 3.19 Straight-Through und Crossover

## Straight-Through

Unterschiedliche Gerätetypen.

Beispiel:

- PC ↔ Switch

---

## Crossover

Gleiche Gerätetypen.

Beispiel:

- Switch ↔ Switch

Moderne Geräte nutzen oft Auto-MDI-X.

---

# 3.20 VLANs

Virtual Local Area Networks.

Erlauben logische Trennung innerhalb eines Switches.

Vorteile:

- Sicherheit
- kleinere Broadcast-Domänen
- bessere Strukturierung

---

# 3.21 Access- und Trunk-Ports

## Access-Port

Gehört genau einem VLAN.

---

## Trunk-Port

Transportiert mehrere VLANs.

---

# 3.22 Spanning Tree Protocol (STP)

Verhindert Schleifen in Netzwerken.

Ohne STP:

- Broadcast-Stürme
- Netzwerkausfälle

---

# 3.23 Broadcast Storm

Ursache:

- Netzwerkschleifen

Folgen:

- massive Netzlast
- Netzwerkausfälle

---

# 3.24 Port Security

Switch-Sicherheitsfunktion.

Kann:

- bestimmte MAC-Adressen erlauben
- Ports sperren
- Angriffe erschweren

---

# 3.25 Switching-Methoden

## Store-and-Forward

- kompletter Frame wird geprüft
- hohe Sicherheit
- Standardverfahren

---

## Cut-Through

- Weiterleitung beginnt früh
- geringere Latenz
- weniger Fehlerkontrolle

---

# 3.26 Layer-2- vs Layer-3-Switch

| Layer 2 | Layer 3 |
|---|---|
| MAC-basiert | Routingfähig |
| Switching | Switching + Routing |
| Kein Routing | Inter-VLAN-Routing möglich |

---

# 3.27 Bedeutung für Fachinformatiker

Ethernet Switching ist zentrale Grundlage für:

- Unternehmensnetzwerke
- Serverkommunikation
- VLAN-Konzepte
- Netzwerksegmentierung
- IT-Sicherheit
- Performanceoptimierung
- Fehlersuche

---

# 4. Verknüpfung der Themen

Die drei Themengebiete hängen direkt zusammen:

| Thema | Zusammenhang |
|---|---|
| Zahlensysteme | Grundlage aller digitalen Daten |
| Netzwerk-Grundlagen | Kommunikation zwischen Geräten |
| Ethernet Switching | Effiziente Weiterleitung im LAN |

Beispiele:

- MAC-Adressen verwenden Hexadezimalzahlen
- IPv4 basiert auf Binärdarstellung
- Subnetzmasken benötigen Binärverständnis
- Switches arbeiten mit MAC-Adressen
- VLANs segmentieren Netzwerke logisch

---

# 5. Prüfungsrelevante Kernpunkte

## Besonders wichtig

### Zahlensysteme

- Binär ↔ Dezimal
- Binär ↔ Hexadezimal
- Bit und Byte
- Stellenwertsystem

### Netzwerk-Grundlagen

- OSI-Modell
- TCP/IP
- MAC vs IP
- DNS
- DHCP
- TCP vs UDP
- Ports
- Subnetzmasken

### Ethernet Switching

- Hub vs Switch
- MAC-Adress-Tabelle
- Broadcast/Unicast/Multicast
- CSMA/CD
- VLANs
- STP
- Ethernet-Frame

---

# 6. Erweiterungen auf FIAE/FISI-Niveau

## 6.1 Warum Hexadezimal in Netzwerken wichtig ist

Hexadezimal ist kompakter und leichter lesbar als Binär.

Beispiel:

```text
11111111 = FF
```

Dadurch eignen sich Hexzahlen besonders für:

- MAC-Adressen
- Speicheradressen
- Debugging
- Low-Level-Programmierung

---

# 6.2 Zusammenhang von Subnetzmasken und Binärsystem

Beispiel:

```text
255.255.255.0
```

Binär:

```text
11111111.11111111.11111111.00000000
```

Die 1 markieren:

- Netzwerkanteil

Die 0 markieren:

- Hostanteil

---

# 6.3 Warum Switches Netzwerke effizienter machen

Switches reduzieren unnötigen Verkehr.

Dadurch:

- weniger Kollisionen
- höhere Geschwindigkeit
- bessere Skalierbarkeit
- stabilere Netzwerke

---

# 6.4 Bedeutung von VLANs in Unternehmen

VLANs ermöglichen Trennung ohne zusätzliche Hardware.

Beispiele:

| VLAN | Bereich |
|---|---|
| VLAN 10 | Verwaltung |
| VLAN 20 | Entwicklung |
| VLAN 30 | Gäste-WLAN |

Vorteile:

- Sicherheit
- Struktur
- reduzierte Broadcasts

---

# 6.5 Praxisbezug Fachinformatik

Diese Themen bilden die Grundlage für:

## Fachinformatiker Systemintegration

- Netzwerkaufbau
- Administration
- Troubleshooting
- VLAN-Konfiguration
- Routing

## Fachinformatiker Anwendungsentwicklung

- Netzwerkprogrammierung
- Serverkommunikation
- APIs
- Socket-Programmierung
- Performanceanalyse

---

# 7. Merksätze

## Zahlensysteme

> 1 Hex-Ziffer entspricht exakt 4 Bit.

> Computer denken binär.

---

## Netzwerk

> MAC-Adresse = Hardwareadresse.

> IP-Adresse = logische Adresse.

---

## Switching

> Switches lernen MAC-Adressen automatisch.

> Router trennen Broadcast-Domänen.

> VLANs segmentieren Netzwerke logisch.

---

# 8. Abschluss

Die behandelten Themen bilden zentrale Grundlagen moderner IT-Systeme.

Ein solides Verständnis dieser Inhalte ist essenziell für:

- Netzwerktechnik
- Systemadministration
- Softwareentwicklung
- IT-Sicherheit
- Servertechnik
- Cloud-Infrastrukturen
- Virtualisierung
- Fehlersuche und Analyse

Insbesondere die Verknüpfung aus:

- Binärlogik
- Protokollen
- Adressierung
- Switching

ist elementar für nahezu jede technische Spezialisierung innerhalb der Informatik.

