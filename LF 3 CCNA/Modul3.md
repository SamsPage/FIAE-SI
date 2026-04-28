# Lernzusammenfassung – Klausur Modul 3

## Grundlagen der Vernetzung

### Was ist ein Netzwerk?
Ein Netzwerk ist die Verbindung von mindestens zwei Geräten, die Daten austauschen können.

Ziele:
- Kommunikation
- Ressourcen gemeinsam nutzen
- Zugriff auf Server
- Internetzugang

### Client und Server
**Client** fordert Dienste an (z. B. Browser, PC, Smartphone)

**Server** stellt Dienste bereit (z. B. Webserver, Mailserver, Dateiserver)

### Netzwerkgeräte
- Switch → verbindet Geräte im gleichen Netzwerk (MAC, Layer 2)
- Router → verbindet verschiedene Netzwerke (IP, Layer 3)
- Access Point → ermöglicht WLAN
- NIC → Netzwerkkarte

---

## Netzwerktypen

- LAN = kleines lokales Netzwerk
- WAN = großes Netzwerk über weite Entfernungen
- WLAN = drahtloses LAN
- PAN = persönliches Netzwerk (z. B. Bluetooth)

---

## Kommunikation & Protokolle

### Was ist ein Protokoll?
Ein Protokoll ist ein festgelegter Satz von Regeln für die Datenübertragung.

Es regelt:
- Format
- Reihenfolge
- Größe
- Fehlerbehandlung
- Adressierung

### Wichtige Protokolle
- HTTP / HTTPS → Webseiten
- DNS → Namen zu IP
- DHCP → automatische IP-Vergabe
- FTP → Dateiübertragung
- SMTP / IMAP / POP3 → E-Mail
- TCP → sichere Übertragung
- UDP → schnelle Übertragung
- IP → Routing
- Ethernet → LAN

---

## TCP vs UDP

### TCP
- sicher
- verbindungsorientiert
- Fehlerkontrolle
- Reihenfolge wichtig

### UDP
- schnell
- verbindungslos
- keine Garantie
- ideal für Streaming

---

## OSI-Modell

### Die 7 Schichten
1. Bitübertragung
2. Sicherung
3. Vermittlung
4. Transport
5. Sitzung
6. Darstellung
7. Anwendung

Merksatz:
**Alle Deutschen Studenten Trinken Verschiedene Sorten Bier**

---

## TCP/IP-Modell

4 Schichten:
- Anwendung
- Transport
- Internet
- Netzwerkzugriff

OSI beschreibt WAS passiert,
TCP/IP beschreibt WIE es praktisch funktioniert.

---

## Datenkapselung

Reihenfolge:
Daten → Segment → Paket → Frame → Bits

Große Daten werden segmentiert:
- schneller
- effizienter
- nur verlorene Teile neu senden

---

## MAC-Adresse vs IP-Adresse

### MAC-Adresse
- physische Hardware-Adresse
- lokal im Netzwerk
- Layer 2

### IP-Adresse
- logische Netzwerkadresse
- für Routing
- Layer 3

Merke:
Switch = MAC  
Router = IP

---

## Running Config vs Startup Config

### Running Config
- aktuelle Konfiguration
- RAM
- nach Neustart weg

### Startup Config
- dauerhaft gespeichert
- NVRAM
- wird beim Start geladen

---

## Verbindungen prüfen

- ping → Erreichbarkeit testen
- tracert / traceroute → Weg durchs Netzwerk
- ipconfig → eigene Netzwerkkonfiguration

---

## Klausurkiller

Nicht verwechseln:
- MAC ≠ IP
- DNS ≠ DHCP
- Switch ≠ Router
- TCP ≠ UDP
- Running ≠ Startup
- LAN ≠ WAN

---

## Ultra-Kurz-Merkliste

Switch = MAC  
Router = IP  
DNS = Name → IP  
DHCP = IP automatisch  
TCP = sicher  
UDP = schnell  
Running = aktuell  
Startup = dauerhaft
