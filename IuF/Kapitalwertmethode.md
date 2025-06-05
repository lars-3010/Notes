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
**Ziel:** Bestimmung des Barwerts aller durch eine Investition verursachten Zahlungen (Ein- und Auszahlungen) zum Entscheidungszeitpunkt (t=0). Der Kapitalwert repräsentiert den zusätzlichen Vermögenszuwachs (in € heute), der durch die Durchführung der Investition im Vergleich zur Anlage des Geldes zum Kalkulationszinssatz erzielt wird.

#### **2.1. Formel**

*   **Name:** Kapitalwert (KW)
*   **Formel (allgemein):**
    $$ KW = \sum_{t=0}^{n} \frac{CF_t}{(1+i)^t} $$
    *Oder, wenn die Anschaffungsauszahlung I₀ explizit als separate Größe in t=0 betrachtet wird (was häufig der Fall ist):*
    $$ KW = -I_0 + \sum_{t=1}^{n} \frac{CF_t}{(1+i)^t} $$
    *Oder auch mit dem Restwert (RWn) am Ende der Nutzungsdauer n als separater Posten im letzten Cashflow oder explizit:*
    $$ KW = -I_0 + \sum_{t=1}^{n} \frac{\text{Laufende } CF_t}{(1+i)^t} + \frac{RW_n}{(1+i)^n} $$
    *Wobei:*
    *   `I₀` = Anschaffungsauszahlung in t=0 (negativer Wert)
    *   `CFt` = Netto-Cashflow (Einzahlungen - Auszahlungen) der Periode t (von t=1 bis n)
    *   `RWn` = Restwert / Liquidationserlös am Ende der Nutzungsdauer n (in Periode n)
    *   `i` = Kalkulationszinssatz
    *   `n` = Nutzungsdauer der Investition
*   **Kurzerklärung:** Der Kapitalwert summiert alle auf heute abgezinsten zukünftigen Zahlungsüberschüsse und zieht davon die heutige Anschaffungsauszahlung ab.

#### **2.2. Entscheidungsregel**

*   **Einzelinvestition:** Eine Investition ist vorteilhaft, wenn ihr **Kapitalwert > 0** ist.
    *   KW > 0: Die Investition erwirtschaftet mehr als die geforderte Mindestverzinsung (i).
    *   KW = 0: Die Investition erwirtschaftet genau die geforderte Mindestverzinsung (i).
    *   KW < 0: Die Investition erwirtschaftet weniger als die geforderte Mindestverzinsung (i) und ist abzulehnen.
*   **Auswahl zwischen mehreren Alternativen:** Wähle die Alternative mit dem **höchsten positiven Kapitalwert**.

#### **2.3. Tabellarisches Rechenschema für die Kapitalwertberechnung**

| Jahr (t) | Zahlung / Cashflow (CFt) (I₀, laufende CFs, RW) | Abzinsungsfaktor (AFt) bei Zinssatz i = (1+i)⁻ᵗ | Barwert (BWt = CFt \* AFt) |
| :------- | :--------------------------------------------- | :----------------------------------------------- | :------------------------- |
| 0        | - I₀                                           | 1,0000                                           | - I₀                       |
| 1        | CF₁                                            | *(aus Tabelle oder berechnet)*                   | BW₁                        |
| 2        | CF₂                                            | *(aus Tabelle oder berechnet)*                   | BW₂                        |
| ...      | ...                                            | ...                                              | ...                        |
| n        | CFn (+ RWn, falls nicht in CFn enthalten)      | *(aus Tabelle oder berechnet)*                   | BWn                        |
|          | **Summe = Kapitalwert (KW)**                   |                                                  | **Σ BWt**                  |

**Wichtige Annahme der Kapitalwertmethode (Prämisse):**
Zwischenzeitlich freiwerdende Mittel (positive Cashflows während der Laufzeit) können zum **Kalkulationszinssatz (i)** wiederangelegt werden. Dies ist ein wichtiger Punkt für den Vergleich mit dem Internen Zinsfuß (siehe Folie 54).
