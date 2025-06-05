---
tags:
  - 🌱
"up::":
  - "[[../../../../Projects/Courses/_Investition und Finanzierung|_Investition und Finanzierung]]"
similar:
leads to:
  - "[[Formelsammlung - dynamische Investitionsverfahren]]"
contradicts:
extends:
implements:
reviewed:
sources:
---
**Grundgedanke:** Betrachtung einer durchschnittlichen Periode, Zeitwert des Geldes wird nicht oder nur vereinfacht berücksichtigt.

---

**1. Kapitalkosten (Grundlage für Kosten- & Gewinnvergleich)**

*Diese Kostenkomponenten fließen in die Gesamtkosten der Kosten- und Gewinnvergleichsrechnung ein.*

**1.1. Durchschnittliche Abschreibung (Ø AfA)**
*   **Zweck:** Erfasst den durchschnittlichen jährlichen Wertverlust der Investition.
*   **Formel:**
    $$ \text{Ø AfA} = \frac{\text{Anschaffungswert (AW) - Restwert (RW)}}{\text{Nutzungsdauer (ND in Jahren)}} $$

**1.2. Durchschnittlicher Kapitaleinsatz (Ø KE) – *Standardfall***
*   **Zweck:** Basis für die Berechnung der kalkulatorischen Zinsen; stellt das durchschnittlich in der Investition gebundene Kapital dar.
*   **Formel:**
    $$ \text{Ø KE} = \frac{\text{Anschaffungswert (AW) + Restwert (RW)}}{2} $$
    *(Hinweis: Geht von linearer Wertminderung bzw. gedanklich gleichmäßiger Tilgung über die Periode aus.)*

**1.3. Kalkulatorische Zinsen (Ø Zinsen)**
*   **Zweck:** Kosten für die Nutzung des in der Investition gebundenen Kapitals (Opportunitätskosten).
*   **Formel:**
    $$ \text{Ø Zinsen} = \text{Ø Kapitaleinsatz (Ø KE)} \times \text{Kalkulationszinssatz (i)} $$
    *(Hinweis: `i` als Dezimalzahl, z.B. 0,08 für 8%)*

---

**2. Kostenvergleichsrechnung**

*Entscheidungskriterium: Wähle die Alternative mit den **minimalen** Kosten (Gesamtkosten bei gleicher Menge, Stückkosten bei unterschiedlicher Menge).*

**2.1. Gesamtkosten pro Periode ($K_{ges}$)**
*   **Zweck:** Ermittlung aller relevanten Kosten einer Alternative in der Durchschnittsperiode.
*   **Formel:**
    $$ K_{ges} = (\text{Ø AfA} + \text{Ø Zinsen})_{\text{Kapitalkosten}} + (K_{fix, betrieblich} + (\text{Menge (x)} \times k_{var}))_{\text{Betriebskosten}} $$
    *Wobei:*
    *   $K_{fix, betrieblich}$ = jährliche fixe Betriebskosten (Miete, Gehälter etc.)
    *   $k_{var}$ = variable Stückkosten (Material/Stück etc.)

**2.2. Stückkosten ($k_{ges}$)**
*   **Zweck:** Vergleich von Alternativen mit unterschiedlicher Produktions-/Absatzmenge (wenn Erlöse pro Stück gleich sind).
*   **Formel:**
    $$ k_{ges} = \frac{K_{ges}}{\text{Menge (x)}} $$

**2.3. Kritische Menge ($m_{kritisch}$) – *zwischen 2 Alternativen A1 und A2***
*   **Zweck:** Ermittlung der Menge, bei der die Gesamtkosten zweier Alternativen gleich sind.
*   **Formel:**
    $$ m_{kritisch} = \frac{K_{F1} - K_{F2}}{k_{v2} - k_{v1}} $$
    *Wobei:*
    *   $K_{F1}, K_{F2}$ = Summe der Fixkosten (Ø AfA + Ø Zinsen + $K_{fix, betrieblich}$) der Alternative 1 und 2.
    *   $k_{v1}, k_{v2}$ = variable Stückkosten der Alternative 1 und 2.
    *   *Hinweis: Nenner positiv wählen ($k_{v2} > k_{v1}$), dann Zähler entsprechend anpassen.*

---

**3. Gewinnvergleichsrechnung**

*Entscheidungskriterium: Wähle die Alternative mit dem **maximalen** Gewinn.*

**3.1. Gesamterlöse pro Periode ($E_{ges}$)**
*   **Zweck:** Ermittlung der gesamten Einnahmen aus dem Verkauf.
*   **Formel:**
    $$ E_{ges} = \text{Absatzmenge (x)} \times \text{Verkaufspreis pro Stück (p)} $$

**3.2. Gewinn pro Periode (G)**
*   **Zweck:** Ermittlung des Periodenerfolgs der Investition.
*   **Formel:**
    $$ G = E_{ges} - K_{ges} $$
    *(Kges wie im Kostenvergleich berechnet)*

**3.3. Break-Even-Menge / Gewinnschwelle ($m_{BEP}$)**
*   **Zweck:** Ermittlung der Absatzmenge, ab der Gewinn erzielt wird (Gewinn = 0).
*   **Deckungsbeitrag pro Stück ($db_{Stück}$):**
    $$ db_{Stück} = p - k_{var} $$
*   **Formel für $m_{BEP}$:**
    $$ m_{BEP} = \frac{K_{fix,gesamt}}{db_{Stück}} = \frac{K_{fix,gesamt}}{p - k_{var}} $$
    *Wobei:*
    *   $K_{fix,gesamt}$ = Summe aller Fixkosten (Ø AfA + Ø Zinsen + $K_{fix, betrieblich}$)

---

**4. Rentabilitätsvergleichsrechnung**

*Entscheidungskriterium: Wähle die Alternative mit der **höchsten** Rentabilität.*

**4.1. Bruttorentabilität (ROI-ähnlich)**
*   **Zweck:** Verzinsung des eingesetzten Kapitals vor Abzug der kalkulatorischen Kapitalkosten.
*   **Formel:**
    $$ \text{Bruttorentabilität} = \frac{\text{Gewinn (G)} + \text{Ø Zinsen (Betrag)}}{\text{Ø Kapitaleinsatz (Ø KE)}} \times 100\% $$
    *(Hinweis: Sollte größer sein als der Kalkulationszinssatz i).*

**4.2. Nettorentabilität**
*   **Zweck:** "Überrendite" nach Abzug der kalkulatorischen Kapitalkosten.
*   **Formel:**
    $$ \text{Nettorentabilität} = \frac{\text{Gewinn (G)}}{\text{Ø Kapitaleinsatz (Ø KE)}} \times 100\% $$
    *(Hinweis: Sollte größer als 0% sein).*

**4.3. *Optional/Verständnis:* ROI-Grundformel & Zerlegung**
*   **ROI:** $ROI = \frac{\text{Gewinn}}{\text{Ø Gesamtkapital}} \times 100\%$
*   **Zerlegung:** $ROI = \underbrace{\left(\frac{\text{Gewinn}}{\text{Umsatz}}\right)}_{\text{Umsatzrentabilität}} \times \underbrace{\left(\frac{\text{Umsatz}}{\text{Ø Gesamtkapital}}\right)}_{\text{Kapitalumschlag}}$

---

**5. Statische Amortisationsrechnung (Pay-Off-Periode)**

*Entscheidungskriterium: Wähle die Alternative mit der **kürzesten** Amortisationsdauer (Risikomaß).*

**5.1. Jährlicher Rückfluss (CF) – *vereinfacht für statischen Kontext***
*   **Zweck:** Liquide Mittel, die pro Periode aus der Investition zurückfließen.
*   **Formel:**
    $$ \text{Jährlicher Rückfluss (CF)} = \text{Gewinn (G)} + \text{Ø AfA} $$
    *(Gewinn G hier typischerweise der Gewinn nach Abschreibungen und nach kalk. Zinsen, wie in der Gewinnvergleichsrechnung ermittelt. AfA wird addiert, da nicht auszahlungswirksam in der Periode).*

**5.2. Amortisationsdauer ($t_A$) – *Fall 1: Konstante jährliche CFs***
*   **Formel:**
    $$ t_A = \frac{\text{Anschaffungsauszahlung (I}_0\text{)}}{\text{Jährlicher Rückfluss (CF)}} $$

**5.3. Amortisationsdauer ($t_A$) – *Fall 2: Unregelmäßige jährliche CFs***
*   **Vorgehen:**
    1.  Kumuliere die jährlichen CFs, bis I₀ erreicht oder überschritten ist.
    2.  Anzahl der vollen Jahre + $\frac{\text{Restbetrag zu Beginn des letzten Amortisationsjahres}}{\text{CF im letzten Amortisationsjahr}}$
