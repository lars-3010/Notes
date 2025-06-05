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
**Ziel:** Entscheidung, zu welchem Zeitpunkt eine bereits genutzte "alte" Anlage durch eine "neue" Anlage ersetzt werden soll, um den Gesamtkapitalwert über einen bestimmten Planungszeitraum oder unendlichen Horizont zu maximieren.
**Anwendung:** Wenn sowohl die alte als auch die neue Anlage über mehrere Perioden Cashflows generieren und Restwerte besitzen.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein (Folie 74 konzeptionell, Übungsaufgaben 18, 19 zeigen die Anwendung):** Die Logik, verschiedene Ersatzstrategien zu definieren und deren Kapitalwerte zu vergleichen. Die Annuitätenmethode kann hier als Hilfsmittel dienen, besonders wenn die neue Anlage unendlich oft identisch wiederbeschafft wird.

#### **2.1. Grundsätzliche Vorgehensweise**

1.  **Definiere einen Planungszeitraum (T):**
    *   **Endlicher Planungshorizont:** Ein festgelegter Zeitraum (z.B. 3 Jahre, wie in ÜA 19 oder deiner Folie 66 zum endlichen Planungshorizont der optimalen Nutzungsdauer, das Prinzip ist ähnlich).
    *   **Unendlicher Planungshorizont:** Man geht davon aus, dass die neue Anlage nach ihrer optimalen Nutzungsdauer immer wieder durch eine identische Anlage ersetzt wird.
2.  **Definiere mögliche Ersatzstrategien:**
    *   Strategie 0: Sofortiger Ersatz der alten Anlage durch die neue.
    *   Strategie 1: Alte Anlage noch 1 Jahr nutzen, dann durch die neue ersetzen.
    *   Strategie k: Alte Anlage noch k Jahre nutzen, dann durch die neue ersetzen.
3.  **Ermittle die Zahlungsreihe für jede Strategie:**
    *   **Phase "Alte Anlage":**
        *   Opportunitätskosten zu Beginn (t=0 bei Strategie 1, 2, ... k): Der heutige Liquidationserlös (Restwert) der alten Anlage, den man aufgibt, wenn man sie weiternutzt (wird oft als negative Zahlung zu Beginn der Weiternutzungsphase angesetzt oder implizit im Vergleich der reinen Weiternutzung vs. sofortigem Ersatz berücksichtigt).
        *   Laufende Cashflows der alten Anlage für die Jahre 1 bis k.
        *   Liquidationserlös (Restwert) der alten Anlage am Ende des Jahres k (Ersatzzeitpunkt).
    *   **Phase "Neue Anlage":**
        *   Anschaffungsauszahlung für die neue Anlage zum Zeitpunkt k.
        *   Laufende Cashflows der neuen Anlage ab Zeitpunkt k+1 bis zum Ende des Planungszeitraums T.
        *   Ggf. Restwert der neuen Anlage am Ende des Planungszeitraums T.
        *   **Bei unendlichem Horizont für die neue Anlage:** Statt der detaillierten Cashflows der neuen Anlage kann man deren **Annuität (AN_neu)** verwenden, die ab dem Ersatzzeitpunkt k anfällt. Der Barwert dieser unendlichen Annuitätenkette (abgezinst auf Zeitpunkt k) ist dann $AN_{neu}/i$.
4.  **Berechne den Gesamtkapitalwert (KW_Strategie) für jede Strategie** zum heutigen Zeitpunkt (t=0).
5.  **Entscheidung:** Wähle die Strategie mit dem **höchsten Gesamtkapitalwert**.

#### **2.2. Zahlungsreihen und Kapitalwertberechnung (Beispielhafter Aufbau für endlichen Horizont oder mit Annuität der neuen Anlage)**

**Annahmen für das Schema:**
*   $CF_{alt,t}$ = Cashflow der alten Anlage im Jahr t ihrer Weiternutzung.
*   $RW_{alt,k}$ = Restwert der alten Anlage, wenn sie nach k Jahren ersetzt wird.
*   $I_{0,neu}$ = Anschaffungsauszahlung der neuen Anlage.
*   $AN_{neu}$ = Annuität der neuen Anlage (berechnet aus deren KW über ihre optimale ND).
*   Planungszeitraum sei hier lang genug oder wir nutzen die Annuität der neuen Anlage.

**Strategie 0: Sofortiger Ersatz**
*   Zahlungsreihe ist einfach die der neuen Anlage (ggf. als Annuitätenkette $AN_{neu}$ oder detaillierte Cashflows).
*   $KW_{S0} = KW_{neu}$ (oder Barwert der Annuitätenkette der neuen Anlage beginnend in t=0).

**Strategie 1: Ersatz nach 1 Jahr**
*   **Zahlungsreihe:**
    *   t=0: (Implizit $RW_{alt,0}$ als Opportunitätskosten, die *nicht* realisiert werden)
    *   t=1: $CF_{alt,1} + RW_{alt,1} - I_{0,neu}$ (Erlöse aus alter Anlage, dann Kauf neue)
    *   t=2: $CF_{neu,1}$ (erster CF der neuen Anlage) oder Beginn der $AN_{neu}$
    *   t=3: $CF_{neu,2}$ oder $AN_{neu}$
    *   ...
*   **KW-Berechnung:** Alle diese Zahlungen auf t=0 abzinsen.
    *   Alternativ und oft einfacher, wenn die $AN_{neu}$ bekannt ist (angenommen, die neue Anlage wird dann unendlich oft wiederbeschafft):
        $ KW_{S1} = \frac{CF_{alt,1} + RW_{alt,1}}{(1+i)^1} + \frac{AN_{neu}/i}{(1+i)^1} - RW_{alt,0} $
        *(Hier wird $RW_{alt,0}$ als Opportunitätskosten direkt abgezogen, und die Erträge der Weiternutzung plus der Barwert der nachfolgenden neuen Anlagenkette werden auf heute abgezinst)*
        *Der Term $AN_{neu}/i$ ist der Barwert einer ewigen Rente der Annuität der neuen Anlage. Dieser Barwert fällt zum Zeitpunkt des Ersatzes an und muss dann noch auf t=0 abgezinst werden.*

**Strategie k: Ersatz nach k Jahren (Allgemeiner Fall mit Annuität der neuen Anlage)**
*   **KW-Berechnung (vereinfacht über Annuitäten, vgl. Folie 75 Schema):**
    Der Barwert der Strategie, die alte Anlage k Jahre zu nutzen und *danach* die neue Anlage (als unendliche Kette) einzusetzen, ist:
    $$ KW_{Sk} = \left( \sum_{t=1}^{k} \frac{CF_{alt,t}}{(1+i)^t} + \frac{RW_{alt,k}}{(1+i)^k} \right) + \frac{AN_{neu}/i}{(1+i)^k} - RW_{alt,0} $$
    *Der erste Klammerausdruck ist der Kapitalwert der Weiternutzung der alten Anlage für k Jahre, wenn man sie heute für $RW_{alt,0}$ verkaufen könnte. Der zweite Term ist der auf heute abgezinste Barwert der "ewigen" neuen Anlage, die nach k Jahren startet.*
    *Die Übungsaufgabe auf deiner Folie 75 verwendet direkt die Annuität der neuen Anlage ($AN_{neu}=60$) und vergleicht die Kapitalwerte verschiedener Halteperioden der alten Anlage.*

**Beispielhafte Tabelle zur Entscheidung (wie auf deiner Folie 75, aber hier als Kapitalwert der Gesamtstrategie):**
*Annahme: $RW_{alt,0}$ (heutiger Restwert der alten Anlage) = 700. $AN_{neu}$ (Annuität der neuen Anlage) = 60. Kalkulationszinssatz i.*

| Ersatz nach (k Jahre) | Zahlungsströme der alten Anlage in den Jahren 1 bis k, inkl. $RW_{alt,k}$ am Ende von k | Barwert der alten Anlage bis k (Teil 1) | Barwert der "ewigen" neuen Kette ab k (Teil 2) $ \frac{AN_{neu}/i}{(1+i)^k} $ | Opportunitätskosten -$RW_{alt,0}$ | **Gesamt-KW der Strategie** |
| :-------------------- | :--------------------------------------------------------------------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------ | :-------------------------------- | :-------------------------- |
| 0 (Sofort)            | -                                                                                        | 0                                        | $AN_{neu}/i$                                                                    | 0 (da direkt KWneu)               | $AN_{neu}/i$ (oder $KW_{neu}$) |
| 1                     | $CF_{alt,1}$, $RW_{alt,1}$                                                               | $BW(CF_{alt,1}+RW_{alt,1})$              | $\frac{AN_{neu}/i}{(1+i)^1}$                                                    | -700                              | **Berechnen**               |
| 2                     | $CF_{alt,1}$, $CF_{alt,2}$, $RW_{alt,2}$                                                 | $BW(CFs_{alt})+BW(RW_{alt,2})$           | $\frac{AN_{neu}/i}{(1+i)^2}$                                                    | -700                              | **Berechnen**               |
| ...                   | ...                                                                                      | ...                                      | ...                                                                             | -700                              | **Berechnen**               |

**Deine Folie 75 vereinfacht das, indem sie direkt die Zahlungsreihe der *Gesamtstrategie* aufstellt:**
*   **1. Sofortiger Ersatz:** Zahlungsreihe ist einfach die Annuität der neuen Anlage ($AN_{neu}$ = 60 in jedem Jahr). Deren Barwert (wenn als ewige Rente ab t=1) wäre $60/i$. (Die Folie zeigt direkt die Annuität, was etwas anders ist als der KW der Strategie, aber zum gleichen Ranking führt, wenn man Annuitäten vergleicht).
*   **2. Ersatz nach einem Jahr:**
    *   t=0: Opportunitätskosten (nicht explizit als -700, sondern wird im KW verrechnet)
    *   t=1: $CF_{alt,1} + RW_{alt,1}$ (z.B. $500+500=1000$ aus altem Restwert und Rückfluss) und *danach* beginnt die Kette der neuen Anlage. Die Folie bildet die Zahlungsreihe:
        *   t=0: -700 (impliziter Verkauf der alten Anlage zum Restwert und Kauf der neuen, wenn man es so interpretiert, dass die 60 die Annuität der neuen ist).
        *   Oder die Folie meint:
            *   Jahr 1: (Rückfluss alt) + (Restwert alt) - (Investition neu) + (Cashflow neu 1) usw.
            *   Das Schema auf Folie 75 scheint eine spezifische Aufgabenstellung abzubilden, wo die Cashflows direkt kombiniert werden.
    *   **Die klarste Methode ist der Vergleich der Gesamt-Kapitalwerte der einzelnen Strategien (Weiterbetrieb 0, 1, 2,... Jahre und DANN Ersatz).**

**Für die Klausur (Fokus):**
*   Verstehe das Prinzip, verschiedene Ersatzzeitpunkte als separate Strategien zu definieren.
*   Sei in der Lage, die Zahlungsreihe für "Weiterbetrieb der alten Anlage für k Jahre + anschließender Ersatz durch neue Anlage" zu skizzieren.
*   Berechne den Kapitalwert für jede dieser Strategien.
*   Die Verwendung der Annuität der neuen Anlage (wenn diese als unendliche Kette gedacht ist) vereinfacht die Berechnung erheblich.
*   Beachte die Opportunitätskosten des heutigen Restwerts der alten Anlage, wenn du die Strategie "Weiterbetrieb" bewertest.
