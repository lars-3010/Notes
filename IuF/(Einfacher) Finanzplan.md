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
**Ziel:** Systematische Erfassung aller Ein- und Auszahlungen, die mit einem Investitionsprojekt und seiner Finanzierung über mehrere Perioden verbunden sind, um das finanzielle Gleichgewicht sicherzustellen und eine Zielgröße (z.B. Endwert des Eigenkapitals, Gesamtprojektendwert) zu ermitteln.

**Grundstruktur eines einfachen Finanzplans (oft tabellarisch):**

1.  **Perioden definieren:** In der Regel Jahresende (t=0, 1, 2, ..., n).
2.  **Zahlungsstrom aus dem Investitionsobjekt:**
    *   Anschaffungsauszahlung (I₀) in t=0 (negativ).
    *   Laufende Cashflows (CFt = Einzahlungen - Auszahlungen aus dem operativen Betrieb des Projekts) in t=1 bis n.
    *   Restwert (RWn) in t=n (positiv).
3.  **Finanzierungsströme:**
    *   **Eigenkapitaleinsatz (EK):** Einzahlung in t=0.
    *   **Fremdkapitalaufnahme (FK):** Einzahlung in t=0 (wenn Aufnahme zu Beginn).
    *   **Fremdkapitalzinsen (Z_FK):** Auszahlungen in t=1 bis n (oder bis Tilgung). Berechnet auf den jeweils offenen FK-Betrag.
    *   **Fremdkapitaltilgung (Til_FK):** Auszahlung(en) zu den vereinbarten Zeitpunkten.
4.  **Saldo pro Periode (vor Disposition):**
    *   Summe aller Ein- und Auszahlungen der Periode (aus Investition und Finanzierung).
    *   $Saldo_t = CF_{Projekt,t} + EK_t + FK_{Aufnahme,t} - Z_{FK,t} - Til_{FK,t}$ (je nachdem was in der Periode anfällt)
5.  **Disposition der Periodensalden (Ausgleichsmaßnahmen):**
    *   **Bei positivem Saldo (Überschuss):** Annahme, dass dieser Betrag angelegt wird (z.B. am Kapitalmarkt zu einem bestimmten Habenzinssatz $i_H$). Dies führt zu einer Auszahlung "Finanzanlage" in der aktuellen Periode und zu einer Einzahlung (Anlagebetrag + Zinsen) in einer späteren Periode.
    *   **Bei negativem Saldo (Defizit):** Annahme, dass dieser Betrag zusätzlich finanziert werden muss (z.B. durch kurzfristigen Kredit zu einem bestimmten Sollzinssatz $i_S$). (Dieser Fall ist in einfachen Plänen seltener detailliert, oft wird versucht, das durch die initiale Finanzierung zu vermeiden).
6.  **Saldo pro Periode (nach Disposition):** Sollte idealerweise Null sein, da alle Überschüsse/Defizite disponiert wurden.
7.  **Ermittlung der Zielgröße:**
    *   **Endwert des Projekts/Eigenkapitals:** Summe aller Werte am Ende der letzten Periode n (z.B. Endwert der Finanzanlagen, verbleibendes EK nach Tilgung).
    *   Manchmal wird auch der Kapitalwert des gesamten Finanzplans berechnet, indem alle Zahlungsströme (inklusive der EK-Einlage als Auszahlung aus Sicht des EK-Gebers und dem Endwert als Einzahlung) auf t=0 abgezinst werden.

**Beispielhaftes Schema eines einfachen Finanzplans (ähnlich ÜA 20, 21a,b und Folie 83-87):**
*Annahmen: Investition, EK-Finanzierung, FK-Finanzierung mit Zinsen, Tilgung FK am Ende, Anlage von Überschüssen zu $i_H$.*

| Position                         | Ende Jahr 0 | Ende Jahr 1         | Ende Jahr 2         | Ende Jahr 3 (Ende ND) |
| :------------------------------- | :---------- | :------------------ | :------------------ | :-------------------- |
| **1. Investitionsobjekt:**       |             |                     |                     |                       |
| Anschaffungsauszahlung           | - I₀        |                     |                     |                       |
| Laufender CF aus Projekt         |             | + CF₁               | + CF₂               | + CF₃                 |
| Restwert Projekt                 |             |                     |                     | + RW₃                 |
| **Summe Investition**            | **- I₀**    | **+ CF₁**           | **+ CF₂**           | **+ CF₃ + RW₃**       |
| **2. Finanzierung:**             |             |                     |                     |                       |
| Eigenkapitaleinsatz              | + EK        |                     |                     |                       |
| Fremdkapitalaufnahme             | + FK        |                     |                     |                       |
| Zinsen auf FK                    |             | - Z₁ ($FK \times i_{FK}$) | - Z₂ ($FK \times i_{FK}$) | - Z₃ ($FK \times i_{FK}$) |
| Tilgung FK                       |             |                     |                     | - FK                  |
| **Summe Finanzierung**           | **+EK +FK** | **- Z₁**            | **- Z₂**            | **- Z₃ - FK**         |
| **3. Saldo vor Disposition**     | **=0** (idealerweise) | **$S_1 = CF_1 - Z_1$** | **$S_2 = CF_2 - Z_2$** | **$S_3 = CF_3+RW_3-Z_3-FK$** |
| **4. Disposition Überschüsse:**  |             |                     |                     |                       |
| Anlage Saldo $S_1$ (zu $i_H$)      |             | - $S_1$ (Auszahlung) |                     |                       |
| Anlage Saldo $S_2$ (zu $i_H$)      |             |                     | - $S_2$ (Auszahlung) |                       |
| Endwert Anlage $S_1$             |             |                     |                     | + $S_1 \times (1+i_H)^2$ |
| Endwert Anlage $S_2$             |             |                     |                     | + $S_2 \times (1+i_H)^1$ |
| **5. Saldo nach Disposition**    | **=0**      | **=0**              | **=0**              | **(bleibt $S_3$)**    |
| **6. Endwertberechnung:**        |             |                     |                     |                       |
| Endwert aus Anlagen              |             |                     |                     | **$S_1(1+i_H)^2 + S_2(1+i_H)$** |
| Saldo aus Periode 3              |             |                     |                     | **$S_3$**             |
| **Gesamt-Endwert des Projekts**  |             |                     |                     | **Summe der beiden oberen** |

**Wichtige Punkte für die Klausur (basierend auf Fokus):**

*   **Saubere Trennung der Zahlungsströme:** Investition, Finanzierung (EK, FK, Zinsen, Tilgung).
*   **Logik des Saldoausgleichs:** Positive Salden werden angelegt (und bringen Zinsen), negative Salden müssten finanziert werden (was Zinskosten verursacht – dieser Teil ist aber oft vereinfacht).
*   **Korrekte Zinsberechnung:** Zinsen auf FK auf den jeweiligen Restbetrag. Zinsen auf Finanzanlagen auf den Anlagebetrag.
*   **Ermittlung des Endwerts:** Was bleibt am Ende der Laufzeit übrig, nachdem alle Verpflichtungen erfüllt und alle Erträge aus Anlagen realisiert wurden?
*   **Folie 88 (Kritische Würdigung):** Verstehe die genannten Vorteile (Anspruchslosigkeit, direkte Ablesbarkeit, Berücksichtigung von Konditionenvielfalt, Aufdeckung von Prämissen, Steuerimplikationen möglich, Grundstruktur für simultane Entscheidungen). Das sind gute Argumentationspunkte.

**Kein Fokus laut deiner Priorisierung auf:**
*   Komplexe, mehrstufige Finanzierungs- oder Anlagestrategien innerhalb des Plans.
*   Detaillierte steuerliche Optimierungen im Plan.
*   Perfekte Abstimmung von Soll- und Habenzinsen zur Maximierung winziger Zinsdifferenzen.

Der Plan soll die grundlegende finanzielle Machbarkeit und den potenziellen Endwert einer Investition unter einfachen Finanzierungs- und Anlagebedingungen darstellen.
