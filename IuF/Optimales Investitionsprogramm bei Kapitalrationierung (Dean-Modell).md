---
tags:
  - 🌱
"up::":
  - "[[../../../Projects/Courses/_Investition und Finanzierung|_Investition und Finanzierung]]"
similar:
leads to:
contradicts:
extends:
implements:
reviewed:
sources:
---
**Ziel:** Auswahl und Zusammenstellung eines Investitionsprogramms aus mehreren voneinander unabhängigen Investitionsprojekten, wenn das zur Verfügung stehende Kapitalbudget begrenzt ist (Kapitalrationierung) und nicht alle potenziell vorteilhaften Projekte realisiert werden können.

**Grundidee:** Projekte werden nach ihrer Vorteilhaftigkeit (Rendite) geordnet und mit den günstigsten verfügbaren Finanzierungsmitteln realisiert, bis entweder das Budget erschöpft ist oder die Rendite des nächsten Projekts niedriger ist als die Kosten der nächsten Finanzierungsquelle.

#### **3.1. Annahmen des (vereinfachten) Dean-Modells**

*   Die Investitionsprojekte sind voneinander unabhängig (die Durchführung eines Projekts beeinflusst nicht die Zahlungsströme eines anderen).
*   Die Projekte sind beliebig teilbar (oder es wird eine Näherungslösung für unteilbare Projekte gesucht, was aber oft den Rahmen sprengt). In Klausuren sind sie oft teilbar oder es passt genau.
*   Es gibt ein begrenztes Kapitalbudget aus Eigen- und/oder Fremdmitteln.
*   Die Finanzierungsmittel haben unterschiedliche Kosten (Zinssätze).

#### **3.2. Vorgehensweise (Dean-Modell)**

1.  **Kapitalnachfragekurve erstellen:**
    *   Berechne für jedes verfügbare Investitionsprojekt dessen **Internen Zinsfuß (IRR)**.
    *   Ordne die Projekte nach **fallendem IRR**.
    *   Trage die Projekte grafisch ab: Auf der X-Achse das kumulierte Investitionsvolumen, auf der Y-Achse der IRR. Es entsteht eine treppenförmige, fallende Kurve.

2.  **Kapitalangebotskurve erstellen:**
    *   Ermittle die Kosten (Sollzinssätze) für die verschiedenen verfügbaren Finanzierungsquellen (z.B. Eigenkapital mit Opportunitätskosten, verschiedene Fremdkapitaltranchen mit unterschiedlichen Zinssätzen).
    *   Ordne die Finanzierungsquellen nach **steigenden Kosten (Zinssätzen)**.
    *   Trage die Finanzierungsquellen grafisch ab: Auf der X-Achse das kumulierte Finanzierungsvolumen, auf der Y-Achse der Zinssatz. Es entsteht eine treppenförmige, steigende Kurve.

3.  **Schnittpunkt und optimales Programm ermitteln:**
    *   Der **Schnittpunkt** der Kapitalnachfrage- und Kapitalangebotskurve bestimmt:
        *   Den **marginalen (Grenz-)Zinssatz (i\*)**: Dies ist der Zinssatz des letzten gerade noch akzeptierten Finanzierungsmittels bzw. die Rendite des letzten gerade noch akzeptierten Projekts.
        *   Das **optimale Investitionsvolumen**.
    *   **Entscheidungsregel für das optimale Programm:**
        *   Realisiere alle Investitionsprojekte, deren **IRR größer oder gleich dem Grenzzinssatz i\*** ist.
        *   Nutze alle Finanzierungsquellen, deren **Kosten kleiner oder gleich dem Grenzzinssatz i\*** sind.

#### **3.3. Tabellarische Methode (oft für Klausuren verwendet, wie ÜA 22 oder Folie 80)**

Anstatt die Kurven explizit zu zeichnen, kann man auch tabellarisch vorgehen:

1.  **Tabelle für Investitionsprojekte:**
    *   Spalten: Projektname, Investitionsvolumen (I₀), Interner Zinsfuß (IRR).
    *   Sortierung: Nach fallendem IRR.
2.  **Tabelle für Finanzierungsquellen:**
    *   Spalten: Finanzierungsquelle, Verfügbares Volumen, Kosten (Zinssatz i_FK).
    *   Sortierung: Nach steigenden Kosten.
3.  **Matching und Bestimmung des optimalen Programms:**
    *   Gehe die sortierte Projektliste von oben (höchster IRR) nach unten durch.
    *   Finanziere jedes Projekt mit den jeweils günstigsten noch verfügbaren Finanzierungsmitteln.
    *   Stoppe, wenn:
        *   Der IRR des nächsten Projekts kleiner ist als die Kosten der nächsten verfügbaren Finanzierungsquelle.
        *   Oder alle profitablen Projekte finanziert sind.
        *   Oder keine Finanzierungsmittel mehr verfügbar sind für das nächste profitable Projekt.

**Beispielhafte Tabelle (Prinzip von Folie 80 und ÜA 22):**

**Investitionsprojekte (sortiert nach IRR absteigend):**

| Projekt | Investitionsvolumen (I₀) | IRR (%) | Kumuliertes I₀ |
| :------ | :----------------------- | :------ | :------------- |
| A       | 4.000                    | 13%     | 4.000          |
| C       | 7.000                    | 11,5%   | 11.000         |
| B       | 2.000                    | 12%     | 13.000         |
| D       | 6.000                    | 10%     | 19.000         |
*(Sortierung korrigiert nach IRR: A, B, C, D)*

| Projekt (korrekt sortiert) | Investitionsvolumen (I₀) | IRR (%) | Kumuliertes I₀ |
| :------------------------- | :----------------------- | :------ | :------------- |
| A                          | 4.000                    | 13%     | 4.000          |
| B                          | 2.000                    | 12%     | 6.000          |
| C                          | 7.000                    | 11,5%   | 13.000         |
| D                          | 6.000                    | 10%     | 19.000         |

**Finanzierungsquellen (sortiert nach Kosten aufsteigend):**

| Quelle | Verfügbares Volumen | Kosten (i_FK) (%) | Kumuliertes Volumen |
| :----- | :------------------ | :---------------- | :------------------ |
| 1      | 8.000               | 9%                | 8.000               |
| 2      | 6.000               | 12,5%             | 14.000              |

**Matching (wie auf Folie 80 nachvollzogen):**

1.  **Projekt A (I₀=4.000, IRR=13%):**
    *   Finanzierung durch Quelle 1 (Kosten 9%). $IRR (13\%) > Kosten (9\%)$. → **Projekt A wird durchgeführt.**
    *   Verbleibendes Volumen Quelle 1: 8.000 - 4.000 = 4.000.
2.  **Projekt B (I₀=2.000, IRR=12%):**
    *   Finanzierung durch Rest Quelle 1 (Kosten 9%). $IRR (12\%) > Kosten (9\%)$. → **Projekt B wird durchgeführt.**
    *   Verbleibendes Volumen Quelle 1: 4.000 - 2.000 = 2.000.
3.  **Projekt C (I₀=7.000, IRR=11,5%):**
    *   Benötigt 7.000.
    *   Verfügbar aus Quelle 1: 2.000 (Kosten 9%). $IRR (11,5\%) > Kosten (9\%)$. → **Teil von C (2.000) wird finanziert.**
    *   Quelle 1 ist erschöpft.
    *   Nächste Finanzierungsquelle: Quelle 2 (Kosten 12,5%).
    *   Für den Rest von Projekt C (5.000): $IRR (11,5\%) < Kosten (12,5\%)$. → **Dieser Teil von C wird NICHT durchgeführt.**
    *   (Auf Folie 80 wurde Projekt C anscheinend nur bis zu 2.000 finanziert, weil dann das Budget der *günstigen* Finanzierung aufgebraucht war und die nächste Finanzierungsquelle (12,5%) teurer als der IRR von C (11,5%) war. Das deutet darauf hin, dass Projekte als teilbar angenommen werden, bis die Grenzkostenbedingung verletzt wird.)

**Optimales Investitionsprogramm laut Folie 80 wäre dann:**
*   Projekt A: 4.000 (finanziert mit Quelle 1 zu 9%)
*   Projekt B: 2.000 (finanziert mit Quelle 1 zu 9%)
*   Projekt C: 2.000 (finanziert mit Quelle 1 zu 9%)
*   Gesamtinvestition: 8.000.
*   Der Grenzzinssatz i\* liegt hier zwischen 11,5% (IRR von C) und 12,5% (Kosten von Quelle 2) bzw. wird durch die Kosten der letzten genutzten Finanzierungsquelle (9%) nach oben und den IRR des ersten *nicht* mehr vollständig durchgeführten profitablen Projekts (11,5% für C) nach unten begrenzt. Der letzte akzeptierte IRR war 11,5% für den Teil von C, finanziert mit 9%. Das ist etwas inkonsistent mit der reinen Schnittpunktlogik, wenn man die nächste Finanzierungsquelle betrachtet.
    Die Logik auf Folie 80 scheint zu sein: Führe Projekte durch, solange IRR > Kosten der *aktuell genutzten Finanzierungsquelle*. Sobald diese Quelle erschöpft ist und die nächste Quelle teurer ist als der IRR des (Rest-)Projekts, stoppe.

**Für die Klausur (Fokus):**
*   Verstehe das Prinzip der Sortierung von Projekten nach IRR (fallend) und Finanzierungsquellen nach Kosten (steigend).
*   Sei in der Lage, die tabellarische Methode anzuwenden, um zu entscheiden, welche Projekte bis zu welchem Umfang durchgeführt werden.
*   Achte auf die Teilbarkeit von Projekten. Wenn Projekte nicht teilbar sind, wird es komplexer (ganz oder gar nicht). In der Regel sind sie in solchen Aufgaben als teilbar zu verstehen oder die Zahlen passen so, dass ganze Projekte finanziert werden können bis zum "Cut-Off".
*   Die grafische Darstellung hilft dem Verständnis, die tabellarische ist oft rechenintensiver, aber präziser für die Lösung.