→ Aufgabe besteht darin, die einzelnen voneinander abhängigen Teilaufgaben in eine sinnvolle, zeitliche und räumliche Reihenfolge zu bringen. Die Ablauforganisation kann in einer EPK (Ereignisgesteuerten Prozesskette) dargestellt werden. Diese Darstellungsform ist berufsübergreifend und wird auch von Kaufmännischen Angestellten verstanden.

**Aufgaben der Ablauforganisation:**
- (Neue) Mitarbeitende verschaffen sich einen guten Überblick über komplexe Arbeitsabläufe
- effiziente Organisation der Arbeitsabläufe

**Grundelemente:**
- Ereignis
- Funktion
- Kontrollfluss (UND, ODER, XOR)

|                            Symbol                            |                                Bedeutung                                 |
| :----------------------------------------------------------: | :----------------------------------------------------------------------: |
|            ![Ereignis](/Bilder/EPK_ereignis.png)             |              **Ereignis**<br>Was passiert?<br>Neuer Zustand              |
|            ![Funktion](/Bilder/EPK_funktion.png)             |              **Funktion**<br>Welche Reaktion, was passiert?              |
|                 ![UND](/Bilder/EPK_UND.png)                  |                   **UND**<br>(Symbol **U**nten offen)                    |
|                ![ODER](/Bilder/EPK_ODER.png)                 | Inklusives **ODER**<br>(A & B oder A oder B)<br>(Symbol **O**ben offen)  |
| ![XOR](/Bilder/EPK_XOR.png)<br>![XOR2](/Bilder/EPK_XOR2.png) |             E**x**klusives Oder (**XOR**)<br>(Entweder Oder)             |
|                             ///                              |                    **(Nachfolgend: Erweitertes EPK)**                    |
|              ![Stelle](/Bilder/EPK_stelle.png)               |           Stelle oder Zuständigkeit<br>(oder Know-How-Quelle)            |
|         ![Information](/Bilder/EPK_information.png)          | Information(squelle)/verwendetes Material<br>oder eingebundene Dokumente |
|       ![EPK Beispiel](/Bilder/EPK_ereignisverweis.png)       |                                                                          |
## Ereignis
→ Was ist im Betrieb passiert?
- Neuer Zustand (zeitpunktbezogen)
- Ereignisse können Auslöser oder Ergebnis von Tätigkeiten sein
- Jede EPK **startet und endet** mit Ereignis

**Form: Sechseckig, rot**
**Formulierung: Sachverhalt + Verb im Perfekt (Produkt ist gefunden, Auftrag ist eingegangen)**

## Funktion
→ Welche Reaktion auf das Ereignis ist erforderlich?
- folgt in der EPK direkt nach dem Ereignis
- Ereignisse und Funktionen **wechseln sich immer ab**

**Form: Rechteck ohne Ecken, Grün**
**Formulierung: Sachverhalt + Verb im Infinitiv (Auftrag bearbeiten, Produkt einpacken)**

## Kontrollfluss (Linien / Pfeile)
→ In welcher Reihenfolge läuft die EPK?
- Zeitlich-logische Reihenfolge
- Ereignisse und Funktionen werden verbunden
- Jedes Ereignis hat **maximal zwei** Kontrollflüsse (ein- und/oder ausgehend)
- Jede Funktion hat **genau zwei** Kontrollflüsse (ein- und ausgehend)
- Kontrollflüsse **überkreuzen sich nicht** und die Linien sind **immer gerade**

## Operatoren (Verzweigungen)
→ Werden verwendet, wenn verschiedene Entscheidungsmöglichkeiten auftreten

**Beispiele:**
- Alternative Arbeitsweisen (Stammkunde oder Neukunde)
- Entscheidungen (Rabatt ja oder nein?)
- Bestimmte Bedingungen (Kunde muss etwas kaufen, um zu bezahlen)

### UND 
- Alle Ereignisse **müssen** eingetroffen sein
- Pfade werden parallel durchlaufen
- Prozess läuft erst weiter, wenn alle Pfade ausgeführt sind

### ODER 
- Mindestes ein von mehreren Ereignissen muss erfüllt sein, oder mindestens eine von mehreren Funktionen wurde ausgeführt
- Ein oder mehrere Pfade werden parallel durchlaufen
- Kein Oder nach einem einzelnen Ereignis. Ereignisse können nicht entscheiden.

### XODER / XOR (exklusives Oder)
- Genau ein Ereignis oder genau eine Funktion muss erfüllt sein
- genau ein Pfad wird ausgewählt
- Kein exklusives Oder nach einem einzelnen Ereignis. Ereignisse können nicht entscheiden.



## Simples Beispiel

![EPK Beispiel Simpel](/Bilder/EPK_beispiel_simpel.png)

## Komplexeres Beispiel

![EPK Beispiel](/Bilder/EPK_beispiel.png)

## Erweitertes Beispiel

![EPK Beispiel 2](/Bilder/EPK_beispiel2.png)


