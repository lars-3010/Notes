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
**Ziel:** Beurteilung der Vorteilhaftigkeit einer Investition anhand der Verzinsung des eingesetzten Kapitals. Auswahl der Alternative mit der höchsten Rentabilität.
**Anwendung:** Besonders wichtig, wenn die zu vergleichenden Investitionsalternativen einen unterschiedlich hohen Kapitaleinsatz erfordern. Reine Gewinn- oder Kostengrößen sind dann oft nicht ausreichend aussagekräftig.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein:** Die Berechnung der Brutto- und Nettorentabilität als Kernkennzahlen. Das Verständnis, warum man zwischen Brutto und Netto unterscheidet.
*   **Konzeptionell wichtig, aber nicht tiefgreifend für die Rechnung:** Das ROI-Konzept (DuPont) wurde bereits kurz angerissen und dient hier primär dem Verständnis, wie Rentabilität analysiert werden kann. Die Detailrechnung des ROI mit all seinen Zerlegungen ist laut Fokus weniger wahrscheinlich als die direkte Berechnung der Investitionsrentabilitäten.

#### **3.1. Grundlegende Größen**

*   **Gewinn pro Periode (G):**
    *   Wird aus der Gewinnvergleichsrechnung übernommen (Erlöse - Gesamtkosten).
    *   Wichtig ist hier oft die Unterscheidung:
        *   **Gewinn *vor* Abzug der kalkulatorischen Zinsen, aber *nach* Abschreibungen:** Dieser wird für die Bruttorentabilität benötigt. In der statischen Gesamtkostenrechnung sind die kalk. Zinsen oft schon Teil der $K_{ges}$. Man muss also ggf. die kalk. Zinsen zum Gewinn (Erlöse - $K_{ges}$) wieder hinzuaddieren oder den Gewinn als (Erlöse - Betriebskosten - Abschreibungen) berechnen.
        *   **Gewinn *nach* Abzug der kalkulatorischen Zinsen und *nach* Abschreibungen:** Dieser wird für die Nettorentabilität benötigt. Entspricht dem G aus der Gewinnvergleichsrechnung, wenn $K_{ges}$ die kalk. Zinsen beinhaltet.
*   **Durchschnittlicher Kapitaleinsatz (Ø KE):**
    *   Wird aus der Kostenvergleichsrechnung übernommen:
        $$ \text{Ø KE} = \frac{\text{Anschaffungswert (AW) + Restwert (RW)}}{2} $$
*   **Kalkulatorische Zinsen (Betrag):**
    *   Wird aus der Kostenvergleichsrechnung übernommen:
        $$ \text{Ø Zinsen (Betrag)} = \text{Ø KE} \times \text{Kalkulationszinssatz (i)} $$

#### **3.2. Berechnung der Rentabilitätskennzahlen**

*   **Investitionsrentabilität – Brutto (vor Abzug der kalkulatorischen Zinsen):**
    *   **Name:** Bruttorentabilität / ROI (oft in diesem Kontext so genannt)
    *   **Formel:**
        $$ \text{Bruttorentabilität} = \frac{\text{Gewinn vor kalk. Zinsen (aber nach AfA)}}{\text{Ø Kapitaleinsatz (Ø KE)}} \times 100\% $$
        *Oder, was oft dasselbe Ergebnis liefert, wenn der "Gewinn" aus der Gewinnvergleichsrechnung bereits die Zinsen als Kosten enthält:*
        $$ \text{Bruttorentabilität} = \frac{\text{Gewinn (nach AfA, nach kalk. Zinsen)} + \text{Ø Zinsen (Betrag)}}{\text{Ø Kapitaleinsatz (Ø KE)}} \times 100\% $$
    *   **Kurzerklärung:** Zeigt, wie sich das durchschnittlich gebundene Kapital insgesamt verzinst, bevor die (kalkulatorischen) Kosten für dieses Kapital selbst abgezogen wurden. Diese Kennzahl sollte **mindestens so hoch sein wie der Kalkulationszinssatz (i)**, damit die Investition die Mindestanforderungen an die Kapitalverzinsung erfüllt.

*   **Investitionsrentabilität – Netto (nach Abzug der kalkulatorischen Zinsen):**
    *   **Name:** Nettorentabilität
    *   **Formel:**
        $$ \text{Nettorentabilität} = \frac{\text{Gewinn nach kalk. Zinsen (und nach AfA)}}{\text{Ø Kapitaleinsatz (Ø KE)}} \times 100\% $$
        *(Der "Gewinn nach kalk. Zinsen" ist hier der Gewinn G, wie er in der Gewinnvergleichsrechnung berechnet wird, vorausgesetzt, die kalk. Zinsen waren Teil der Gesamtkosten Kges).*
    *   **Kurzerklärung:** Zeigt die "Überrendite" der Investition, also die Verzinsung, die über die Deckung der Opportunitätskosten des Kapitals (kalkulatorische Zinsen) hinausgeht. Diese Kennzahl sollte **größer als 0%** sein, damit die Investition vorteilhaft ist (d.h. mehr erwirtschaftet als die geforderte Mindestverzinsung).

*   **Umsatzrentabilität (als Teil des ROI-Verständnisses, aber nicht Hauptfokus der Rentabilitäts*vergleichs*rechnung):**
    *   **Name:** Umsatzrentabilität
    *   **Formel:**
        $$ \text{Umsatzrentabilität} = \frac{\text{Gewinn (Definition beachten, oft vor Zinsen)}}{\text{Umsatz (Gesamterlöse)}} \times 100\% $$
    *   **Kurzerklärung:** Wie viel Prozent des Umsatzes als Gewinn verbleiben.

*   **Kapitalumschlag (als Teil des ROI-Verständnisses):**
    *   **Name:** Kapitalumschlag
    *   **Formel:**
        $$ \text{Kapitalumschlag} = \frac{\text{Umsatz (Gesamterlöse)}}{\text{Ø Kapitaleinsatz (Ø KE)}} $$
    *   **Kurzerklärung:** Wie oft das eingesetzte Kapital pro Periode durch den Umsatz "umgeschlagen" wird.

**Entscheidungskriterium Rentabilitätsvergleich:**
Wähle die Alternative mit der **höchsten (Brutto- oder Netto-)Rentabilität**. Die Bruttorentabilität sollte > Kalkulationszinssatz sein, die Nettorentabilität sollte > 0% sein.

**Tabellarisches Rechenschema für den Rentabilitätsvergleich (basierend auf Ergebnissen aus Kosten- und Gewinnvergleich):**

| Position                                    | Alternative A                                  | Alternative B                                  |
| :------------------------------------------ | :--------------------------------------------- | :--------------------------------------------- |
| Gewinn nach kalk. Zinsen (aus Gewinnvergl.) | $G_A$                                          | $G_B$                                          |
| Ø Kalkulatorische Zinsen (Betrag)           | $Z_A$                                          | $Z_B$                                          |
| Gewinn vor kalk. Zinsen                     | $G_A + Z_A$                                    | $G_B + Z_B$                                    |
| Ø Kapitaleinsatz (aus Kostenvergl.)         | $ØKE_A$                                        | $ØKE_B$                                        |
| **Bruttorentabilität (%)**                  | **$(G_A + Z_A) / ØKE_A \times 100$**           | **$(G_B + Z_B) / ØKE_B \times 100$**           |
| **Nettorentabilität (%)**                   | **$G_A / ØKE_A \times 100$**                   | **$G_B / ØKE_B \times 100$**                   |
| *Vergleich mit Kalkulationszinssatz i*      | *Brutto > i ? / Netto > 0 ?*                   | *Brutto > i ? / Netto > 0 ?*                   |
