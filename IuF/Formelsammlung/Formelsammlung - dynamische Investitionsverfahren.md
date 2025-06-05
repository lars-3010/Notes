---
tags:
  - 🌱
"up::":
  - "[[../../../../Projects/Courses/_Investition und Finanzierung|_Investition und Finanzierung]]"
  - "[[Formelsammlung - statische Investitionsverfahren]]"
similar:
leads to:
  - "[[Formelsammlung - Optimierungsansätze & Sonderfälle]]"
contradicts:
extends:
implements:
reviewed:
sources:
---
**Grundgedanke:** Berücksichtigen den Zeitwert des Geldes. Zukünftige Zahlungen werden auf einen einheitlichen Zeitpunkt (meist t=0) abgezinst.

---

**1. Grundlagen: Zeitwert des Geldes**

**1.1. Abzinsungsfaktor (AFt) / Diskontierungsfaktor**
*   **Zweck:** Faktor, um eine zukünftige Zahlung auf ihren heutigen Wert zu bringen.
*   **Formel:**
    $$ AF_t = \frac{1}{(1+i)^t} = (1+i)^{-t} $$
    *Wobei `i` = Kalkulationszinssatz, `t` = Anzahl Perioden.*

**1.2. Barwert (BWt) einer einzelnen zukünftigen Zahlung ($CF_t$)**
*   **Zweck:** Heutiger Wert einer zukünftigen Zahlung.
*   **Formel:**
    $$ BW_t = CF_t \times AF_t = \frac{CF_t}{(1+i)^t} $$

---

**2. Kapitalwertmethode (KW / NPV)**

*Entscheidungskriterium: Investition vorteilhaft, wenn **KW > 0**. Bei Alternativen wähle die mit dem **höchsten positiven KW**.*

**2.1. Kapitalwert (KW)**
*   **Zweck:** Misst den Vermögenszuwachs (in € heute) durch die Investition über die reine Verzinsung zum Kalkulationszinssatz hinaus.
*   **Formel:**
    $$ KW = -I_0 + \sum_{t=1}^{n} \frac{CF_t}{(1+i)^t} $$
    *(Oder, falls der Restwert $RW_n$ separat betrachtet wird:*
    $$ KW = -I_0 + \sum_{t=1}^{n} \frac{\text{Laufender } CF_t}{(1+i)^t} + \frac{RW_n}{(1+i)^n} $$
    *Wobei $I_0$ = Anschaffungsauszahlung in t=0, $CF_t$ = Netto-Cashflow Periode t, $RW_n$ = Restwert am Ende der Nutzungsdauer n).*
*   **Tabellarisches Rechenschema:**

    | Jahr (t) | Zahlung / Cashflow ($CF_t$) (I₀, laufende CFs, RW) | Abzinsungsfaktor ($AF_t$) bei i | Barwert ($BW_t = CF_t \times AF_t$) |
    | :------- | :--------------------------------------------- | :---------------------------- | :-------------------------------- |
    | 0        | -$I_0$                                         | 1,0000                        | -$I_0$                            |
    | 1        | $CF_1$                                         | $(1+i)^{-1}$                  | $BW_1$                            |
    | 2        | $CF_2$                                         | $(1+i)^{-2}$                  | $BW_2$                            |
    | ...      | ...                                            | ...                           | ...                               |
    | n        | $CF_n$ (+ $RW_n$, falls nicht in $CF_n$)       | $(1+i)^{-n}$                  | $BW_n$                            |
    |          | **Summe = Kapitalwert (KW)**                   |                               | **$\sum BW_t$**                   |

**2.2. Wichtige Annahme (Prämisse):** Zwischenzeitlich freiwerdende Mittel werden zum **Kalkulationszinssatz (i)** wiederangelegt.

---

**3. Interner Zinsfuß Methode (IRR)**

*Entscheidungskriterium: Investition vorteilhaft, wenn **IRR > Kalkulationszinssatz (i)**. Bei Alternativen wähle die mit dem **höchsten IRR** (Vorsicht: Prämissenkonflikt!).*

**3.1. Grundgleichung (KW(IRR) = 0)**
*   **Zweck:** Der IRR ist der Zinssatz, bei dem der Kapitalwert der Investition Null ist; die effektive Rendite des Projekts.
*   **Formel:**
    $$ 0 = -I_0 + \sum_{t=1}^{n} \frac{CF_t}{(1+IRR)^t} $$

**3.2. Lineare Interpolationsformel für IRR**
*   **Zweck:** Näherungsweise Berechnung des IRR, wenn zwei Zinssätze $i_1$ (mit $KW_1 > 0$) und $i_2$ (mit $KW_2 < 0$) bekannt sind.
*   **Formel:**
    $$ IRR \approx i_1 - KW_1 \times \frac{i_2 - i_1}{KW_2 - KW_1} $$
    *(Oder: $ IRR \approx i_1 + \frac{KW_1}{KW_1 - KW_2} \times (i_2 - i_1) $)*
    *Hinweis: $KW_1$ ist positiv, $KW_2$ ist negativ. $i_1$ und $i_2$ sollten nicht zu weit auseinanderliegen.*

**3.3. *Sonderfall:* IRR über Rentenbarwertfaktor (RBF) bei konstanten jährlichen Rückflüssen (R)**
*   **Formel:**
    $$ RBF(IRR, n) = \frac{I_0}{R} $$
    *Vorgehen: Wert $I_0/R$ berechnen, dann in RBF-Tabelle bei Nutzungsdauer n den zugehörigen Zinssatz (IRR) suchen (ggf. interpolieren).*

**3.4. Wichtige Annahme (Prämisse):** Zwischenzeitlich freiwerdende Mittel werden zum **Internen Zinsfuß (IRR) des Projekts** wiederangelegt.

---

**4. Annuitätenmethode**

*Entscheidungskriterium: Investition vorteilhaft, wenn **AN > 0**. Bei Alternativen (bes. unterschiedl. ND) wähle die mit der **höchsten positiven AN**.*

**4.1. Kapitalwiedergewinnungsfaktor (KWF / ANF)**
*   **Zweck:** Faktor zur Umrechnung eines Kapitalwerts in eine gleichbleibende jährliche Zahlung (Annuität).
*   **Formel:**
    $$ KWF(i, n) = ANF(i, n) = \frac{i \times (1+i)^n}{(1+i)^n - 1} $$

**4.2. Rentenbarwertfaktor (RBF)**
*   **Zweck:** Faktor zur Umrechnung einer gleichbleibenden jährlichen Zahlung (Annuität) in einen Kapitalwert. Kehrwert des KWF.
*   **Formel:**
    $$ RBF(i, n) = \frac{(1+i)^n - 1}{i \times (1+i)^n} $$

**4.3. Annuität (AN) aus Kapitalwert (KW)**
*   **Zweck:** Gleichmäßiger jährlicher Überschuss der Investition über die gesamte Nutzungsdauer.
*   **Formel:**
    $$ AN = KW \times KWF(i, n) \quad \text{oder} \quad AN = \frac{KW}{RBF(i, n)} $$

---

**5. Dynamische Amortisationsrechnung**

*Entscheidungskriterium: Kürzere dynamische Amortisationsdauer ist tendenziell besser (Risikomaß).*

**5.1. Vorgehen**
*   **Zweck:** Zeitraum, bis die Anschaffungsauszahlung durch die *Barwerte* der Rückflüsse gedeckt ist.
*   **Berechnung:**
    1.  Berechne die Barwerte (BWt) der jährlichen $CF_t$.
    2.  Kumuliere die $BW_t$, bis $I_0$ erreicht oder überschritten ist.
    3.  Interpolation für das letzte Jahr:
        $ \text{Anteil letztes Jahr} = \frac{\text{Noch zu deckender Barwert zu Beginn des letzten Jahres}}{\text{Barwert des CF im letzten Amortisationsjahr}} $
        $ t_{A,dyn} = (\text{Volle Jahre}) + \text{Anteil letztes Jahr} $
*   **Tabellarisches Rechenschema:**

    | Jahr (t) | $CF_t$ | $AF_t$ bei i | $BW_t$   | Kumulierter $BW$ der CFs (ab t=1) |
    | :------- | :----- | :----------- | :------- | :-------------------------------- |
    | 0        | -$I_0$ | 1,0000       | -$I_0$   |                                   |
    | 1        | $CF_1$ | ...          | $BW_1$   | $BW_1$                            |
    | 2        | $CF_2$ | ...          | $BW_2$   | $BW_1 + BW_2$                     |
    | ...      | ...    | ...          | ...      | ... (bis $\ge I_0$)               |

---

**6. Prämissenkonflikt KW vs. IRR (Folie 54!!) – *Kurze Stichpunkte***

*   **Unterschiedliche Wiederanlageprämissen:**
    *   KW-Methode: Rückflüsse werden zum Kalkulationszinssatz **(i)** wiederangelegt. (Meist als realistischer angesehen).
    *   IRR-Methode: Rückflüsse werden zum **Internen Zinsfuß (IRR) des Projekts** wiederangelegt. (Kann unrealistisch sein, wenn IRR sehr hoch).
*   **Empfehlung bei Konflikt (unterschiedliche Rangfolge der Projekte):**
    *   Der **Kapitalwertmethode (KW)** wird meist der Vorzug gegeben, da sie den absoluten Vermögenszuwachs in € misst und eine marktkonformere Wiederanlageprämisse hat.
*   **Ursachen für Konflikte:** Unterschiedliche Investitionshöhen, unterschiedliche Laufzeiten, unterschiedliche Zahlungsstromprofile.
