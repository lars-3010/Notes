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
**Ziel:** Ermittlung des Zinssatzes (der Rendite), bei dem der Kapitalwert einer Investition genau Null ist. Der IRR gibt also die effektive jährliche Verzinsung des jeweils in der Investition gebundenen Kapitals an.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein:** Das Verständnis der Definition (KW=0), die Berechnung mittels linearer Interpolation (Standardverfahren in Klausuren, wenn keine direkte Lösung möglich) und die Entscheidungsregel.
*   **Wichtig für Verständnis:** Der Prämissenkonflikt mit der KW-Methode.

#### **3.1. Definition und Grundgleichung**

*   **Name:** Interner Zinsfuß (IRR oder r)
*   **Definition:** Der IRR ist derjenige Diskontierungszinssatz, bei dem die Summe der Barwerte aller Zahlungsüberschüsse (Cashflows) gleich der Anschaffungsauszahlung ist, d.h. der Kapitalwert der Investition ist Null.
*   **Grundgleichung:**
    $$ KW(IRR) = -I_0 + \sum_{t=1}^{n} \frac{CF_t}{(1+IRR)^t} = 0 $$
    *Oder umgeformt:*
    $$ I_0 = \sum_{t=1}^{n} \frac{CF_t}{(1+IRR)^t} $$
    *Wobei:*
    *   `I₀` = Anschaffungsauszahlung in t=0
    *   `CFt` = Netto-Cashflow (Einzahlungen - Auszahlungen) der Periode t
    *   `n` = Nutzungsdauer der Investition
    *   `IRR` = Interner Zinsfuß (der gesuchte Wert)
*   **Kurzerklärung:** Der IRR ist die "interne" Rendite des Projekts selbst, unabhängig von einem extern vorgegebenen Kalkulationszinssatz.

#### **3.2. Berechnung des IRR**

Die direkte analytische Lösung der IRR-Gleichung ist oft nur bei sehr einfachen Zahlungsreihen (z.B. nur zwei Perioden) möglich. In der Praxis und in Klausuren wird der IRR meist durch Iteration (systematisches Probieren) oder lineare Interpolation ermittelt.

*   **Lineare Interpolation (Standardverfahren in Klausuren):**
    *   **Voraussetzung:** Man benötigt zwei Zinssätze ($i_1$ und $i_2$), wobei der eine zu einem positiven Kapitalwert ($KW_1 > 0$) und der andere zu einem negativen Kapitalwert ($KW_2 < 0$) führt. Der IRR muss zwischen $i_1$ und $i_2$ liegen.
    *   **Formel (siehe auch deine Formelsammlung Folie 48):**
        $$ IRR \approx i_1 - KW_1 \times \frac{i_2 - i_1}{KW_2 - KW_1} $$
        *Oder, oft intuitiver und weniger fehleranfällig (da $KW_2$ negativ ist):*
        $$ IRR \approx i_1 + \frac{KW_1}{KW_1 - KW_2} \times (i_2 - i_1) $$
        *(Beide Formeln führen zum selben Ergebnis, wenn $KW_1 > 0$ und $KW_2 < 0$ sind. Achte auf die korrekten Vorzeichen!)*
    *   *Wobei:*
        *   `i₁` = Zinssatz, der zu $KW_1 > 0$ führt (der niedrigere der beiden Versuchszinssätze)
        *   `i₂` = Zinssatz, der zu $KW_2 < 0$ führt (der höhere der beiden Versuchszinssätze)
        *   `KW₁` = Positiver Kapitalwert bei Zinssatz `i₁`
        *   `KW₂` = Negativer Kapitalwert bei Zinssatz `i₂`
    *   **Kurzerklärung:** Man nähert sich dem IRR, indem man eine Gerade zwischen den beiden Punkten $(i_1, KW_1)$ und $(i_2, KW_2)$ legt und deren Nullstelle berechnet. Für eine gute Näherung sollten $i_1$ und $i_2$ nicht zu weit auseinanderliegen.

*   **Sonderfall: Gleichförmige Zahlungsreihe (konstante jährliche Rückflüsse R):**
    *   Wenn eine Investition $I_0$ für $n$ Jahre konstante jährliche Rückflüsse $R$ erbringt (und keinen Restwert hat), gilt am IRR-Punkt:
        $$ I_0 = R \times RBF(IRR, n) $$
        Daraus folgt:
        $$ RBF(IRR, n) = \frac{I_0}{R} $$
    *   **Vorgehen:**
        1.  Berechne den Wert $I_0/R$.
        2.  Suche in einer Rentenbarwertfaktortabelle (RBF-Tabelle) in der Zeile für die Nutzungsdauer $n$ den RBF-Wert, der $I_0/R$ am nächsten kommt.
        3.  Der zugehörige Zinssatz in der Spaltenüberschrift ist dann der (ungefähre) IRR. Ggf. muss auch hier interpoliert werden, wenn der Wert genau zwischen zwei Tabellenwerten liegt.
    *   **Kurzerklärung:** Vereinfachte IRR-Findung bei konstanten Rückflüssen über RBF-Tabellen.

#### **3.3. Entscheidungsregel**

*   **Einzelinvestition:** Eine Investition ist vorteilhaft, wenn ihr **Interner Zinsfuß (IRR) > Kalkulationszinssatz (i)** ist.
    *   IRR > i: Die Investition verzinst das gebundene Kapital höher als die geforderte Mindestrendite.
    *   IRR = i: Die Investition verzinst das gebundene Kapital genau mit der geforderten Mindestrendite (entspricht KW=0).
    *   IRR < i: Die Investition verzinst das gebundene Kapital niedriger als die geforderte Mindestrendite.
*   **Auswahl zwischen mehreren Alternativen:** Wähle die Alternative mit dem **höchsten Internen Zinsfuß**, vorausgesetzt dieser liegt über dem Kalkulationszinssatz. **Aber Vorsicht: Prämissenkonflikt mit KW beachten!** (siehe Folie 54 und unser nächster Punkt).

#### **3.4. Tabellarisches Rechenschema für die IRR-Ermittlung (zur Berechnung von KW₁ und KW₂ für die Interpolation)**

Verwende das gleiche Schema wie bei der Kapitalwertberechnung, aber setze jeweils $i_1$ und $i_2$ als Zinssatz ein, um $KW_1$ und $KW_2$ zu erhalten.

| Schritt     | Versuchszinssatz (i) | Jahr (t) | Zahlung (CFt) | AFt bei i       | BWt bei i       | Kapitalwert (KW) bei i |
| :---------- | :------------------- | :------- | :------------ | :-------------- | :-------------- | :--------------------- |
| **Für KW₁** | $i_1$ (z.B. 8%)      | 0        | -I₀           | 1,0000          | -I₀             |                        |
|             |                      | 1        | CF₁           | $(1+i_1)^{-1}$  | $BW_{1,i1}$     |                        |
|             |                      | ...      | ...           | ...             | ...             |                        |
|             |                      | n        | CFn (+RWn)    | $(1+i_1)^{-n}$  | $BW_{n,i1}$     | **$KW_1$ (sollte >0 sein)** |
| **Für KW₂** | $i_2$ (z.B. 10%)     | 0        | -I₀           | 1,0000          | -I₀             |                        |
|             |                      | 1        | CF₁           | $(1+i_2)^{-1}$  | $BW_{1,i2}$     |                        |
|             |                      | ...      | ...           | ...             | ...             |                        |
|             |                      | n        | CFn (+RWn)    | $(1+i_2)^{-n}$  | $BW_{n,i2}$     | **$KW_2$ (sollte <0 sein)** |

**Wichtige Annahme der IRR-Methode (Prämisse):**
Zwischenzeitlich freiwerdende Mittel (positive Cashflows während der Laufzeit) können zum **Internen Zinsfuß (IRR) des Projekts selbst** wiederangelegt werden. Dies ist oft eine unrealistischere Annahme als die der KW-Methode, besonders wenn der IRR sehr hoch ist.
