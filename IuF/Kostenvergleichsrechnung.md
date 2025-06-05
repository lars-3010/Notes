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
reviewed: 2025-06-02T19:54:48+02:00
sources:
---
**Ziel:** Auswahl der Investitionsalternative mit den geringsten (durchschnittlichen) Gesamtkosten pro Periode oder pro Stück.
**Anwendung:** Sinnvoll, wenn die Erlöse der verglichenen Alternativen identisch sind oder schwer zu quantifizieren sind.


#### **1.1. Ermittlung der relevanten Kostenkomponenten pro Periode**

**a) Kapitalkosten (Abschreibungen und kalkulatorische Zinsen):**

*   **Durchschnittliche Abschreibungen (lineare Methode):**
    *   **Name:** Durchschnittliche Abschreibung (Ø AfA)
    *   **Formel:**
        $$ \text{Ø AfA} = \frac{\text{Anschaffungswert (AW) - Restwert (RW)}}{\text{Nutzungsdauer (ND in Jahren)}} $$
    *   **Kurzerklärung:** Erfasst den durchschnittlichen jährlichen Wertverlust der Investition. Der Restwert ist der geschätzte Wert am Ende der Nutzungsdauer.

*   **Durchschnittlicher Kapitaleinsatz (Ø KE):**
    *   **Name:** Durchschnittlicher Kapitaleinsatz
    *   **Formel (Standardfall: Abschreibung/Tilgung erfolgt gedanklich gleichmäßig über die Periode oder am Jahresende für die statische Betrachtung):**
        $$ \text{Ø KE} = \frac{\text{Anschaffungswert (AW) + Restwert (RW)}}{2} $$
    *   **Formel (Alternative, seltener in Grundaufgaben, wenn explizit kontinuierliche Tilgung über die Lebensdauer gemeint ist und der RW=0 wäre):**
        $$ \text{Ø KE} = \frac{\text{Anschaffungswert (AW)}}{2} $$
        *(Hinweis: Die erste Formel ist für Klausuren meist die sicherere Annahme, wenn nichts anderes spezifiziert ist, da sie den durchschnittlich gebundenen Wert über die Nutzungsdauer besser abbildet, wenn ein Restwert existiert.)*
    *   **Kurzerklärung:** Das durchschnittlich in der Investition gebundene Kapital, auf das Zinsen berechnet werden.

*   **Kalkulatorische Zinsen:**
    *   **Name:** Durchschnittliche kalkulatorische Zinsen (Ø Zinsen)
    *   **Formel:**
        $$ \text{Ø Zinsen} = \text{Ø Kapitaleinsatz (Ø KE)} \times \text{Kalkulationszinssatz (i)} $$
    *   **Kurzerklärung:** Kosten für die Nutzung des in der Investition gebundenen Kapitals (Opportunitätskosten). Der Kalkulationszinssatz (i) wird als Dezimalzahl eingesetzt (z.B. 8% = 0,08).

**b) Betriebskosten:**

*   **Fixe Betriebskosten (Kfix, betrieblich):**
    *   **Definition:** Kosten, die unabhängig von der Produktions-/Absatzmenge anfallen (z.B. Miete für Maschinenhalle, Gehälter für festangestelltes Personal, Wartungspauschalen). Werden pro Periode (z.B. pro Jahr) angegeben.

*   **Variable Betriebskosten (Kvar):**
    *   **Definition:** Kosten, die direkt von der Produktions-/Absatzmenge (x oder m) abhängen.
    *   **Formel (Gesamte variable Kosten pro Periode):**
        $$ K_{var, gesamt} = \text{Menge (x)} \times \text{variable Stückkosten (kvar)} $$
    *   **Komponenten der variablen Stückkosten (kvar):** Können z.B. Materialkosten/Stück, Energiekosten/Stück, Fertigungslöhne/Stück sein.

#### **1.2. Berechnung der Gesamtkosten und Stückkosten**

*   **Gesamtkosten pro Periode (Kges):**
    *   **Name:** Gesamtkosten pro Periode
    *   **Formel:**
        $$ K_{ges} = \text{Ø AfA} + \text{Ø Zinsen} + K_{fix, betrieblich} + K_{var, gesamt} $$
    *   **Kurzerklärung:** Summe aller relevanten Kosten, die einer Investitionsalternative in der betrachteten Durchschnittsperiode zugerechnet werden.

*   **Durchschnittliche Stückkosten (kges):**
    *   **Name:** Durchschnittliche Stückkosten
    *   **Formel:**
        $$ k_{ges} = \frac{K_{ges}}{\text{Menge (x)}} $$
    *   **Kurzerklärung:** Kosten pro produzierter/abgesetzter Einheit. Wichtig für den Vergleich, wenn die Alternativen unterschiedliche Produktionsmengen (Kapazitäten) haben.

#### **1.3. Kritische Menge / Auslastung (bei Vergleich von zwei Alternativen mit unterschiedlichen Kostenstrukturen)**

*   **Name:** Kritische Menge (mkritisch)
*   **Formel (Schnittpunkt zweier Kostenfunktionen Kges1 = Kges2):**
    $$ m_{kritisch} = \frac{K_{F1} - K_{F2}}{k_{v2} - k_{v1}} $$
    *Wobei:*
    *   $K_{F1}, K_{F2}$ = Summe der Fixkosten (Ø AfA + Ø Zinsen + Kfix, betrieblich) der Anlage 1 und 2
    *   $k_{v1}, k_{v2}$ = variable Stückkosten der Anlage 1 und 2
*   **Kurzerklärung:** Die Produktions-/Absatzmenge, bei der die Gesamtkosten beider Alternativen gleich hoch sind.
    *   Unterhalb der kritischen Menge ist die Alternative mit den geringeren Fixkosten günstiger.
    *   Oberhalb der kritischen Menge ist die Alternative mit den geringeren variablen Stückkosten günstiger.

**Entscheidungskriterium Kostenvergleich:**
Wähle die Alternative mit den **minimalen Gesamtkosten** (wenn Produktionsmenge gleich) bzw. den **minimalen Stückkosten** (wenn Produktionsmenge unterschiedlich). Bei unterschiedlichen Mengen und schneidenden Kostenfunktionen ist die kritische Menge relevant.

**Tabellarisches Rechenschema für den Kostenvergleich (Beispiel für 2 Alternativen):**

| Kostenart                       | Alternative A (€)                                      | Alternative B (€)                                      |
| :------------------------------ | :----------------------------------------------------- | :----------------------------------------------------- |
| **1. Kapitalkosten:**           |                                                        |                                                        |
| Anschaffungswert (AW)           | *gegeben*                                              | *gegeben*                                              |
| Restwert (RW)                   | *gegeben*                                              | *gegeben*                                              |
| Nutzungsdauer (ND)              | *gegeben*                                              | *gegeben*                                              |
| Ø Abschreibung (AfA)            | (AW - RW) / ND                                         | (AW - RW) / ND                                         |
| Ø Kapitaleinsatz (KE)           | (AW + RW) / 2                                          | (AW + RW) / 2                                          |
| Kalkulationszinssatz (i)        | *gegeben*                                              | *gegeben*                                              |
| Ø Zinsen                        | Ø KE \* i                                              | Ø KE \* i                                              |
| **Summe Kapitalkosten**         | **Ø AfA + Ø Zinsen**                                   | **Ø AfA + Ø Zinsen**                                   |
| **2. Betriebskosten:**          |                                                        |                                                        |
| Fixe Betriebskosten p.a.        | *gegeben*                                              | *gegeben*                                              |
| Menge (x) p.a.                  | *gegeben*                                              | *gegeben*                                              |
| Variable Stückkosten (kvar)     | *gegeben*                                              | *gegeben*                                              |
| Variable Gesamtkosten p.a.      | x \* kvar                                              | x \* kvar                                              |
| **Summe Betriebskosten**        | **Fixe Betr.kost. + Var. Ges.kost.**                   | **Fixe Betr.kost. + Var. Ges.kost.**                   |
| **3. Gesamtkosten p.a. (Kges)** | **Summe KapitalK + Summe BetriebsK**                     | **Summe KapitalK + Summe BetriebsK**                     |
| **4. Stückkosten (kges)**       | **Kges / x**  *(Nur relevant bei unterschiedl. Mengen)* | **Kges / x**  *(Nur relevant bei unterschiedl. Mengen)* |
