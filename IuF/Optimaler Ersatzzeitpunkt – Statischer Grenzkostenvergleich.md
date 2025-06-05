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
**Ziel:** Entscheidung, ob eine bereits genutzte "alte" Anlage für eine weitere Periode (z.B. ein weiteres Jahr) weiterbetrieben oder durch eine "neue" Anlage ersetzt werden soll. Es ist ein *kurzfristiger, periodenbezogener Vergleich*.

**Grundregel:** Ein Ersatz der alten Anlage durch die neue Anlage ist dann wirtschaftlich sinnvoll, wenn die **Durchschnittskosten der neuen Anlage** für die kommende Periode geringer sind als die **Grenzkosten (zusätzlichen Kosten) des Weiterbetriebs der alten Anlage** für genau diese kommende Periode.

**Entscheidung:** Ersetzen, wenn $ \text{ØKosten}_{neu} < \text{Grenzkosten}_{alt, nächste Periode} $

#### **A. Berechnung der Grenzkosten der alten Anlage für die nächste Periode ($GK_{alt,nächste Periode}$)**

Diese Kosten fallen *zusätzlich* an, wenn die alte Anlage ein weiteres Jahr betrieben wird, anstatt sie *sofort* zu verkaufen.

1.  **Opportunitätskosten des Wertverlusts (Kapitalverzehr):**
    *   Differenz zwischen dem Liquidationserlös (Restwert) heute und dem erwarteten Liquidationserlös in einem Jahr.
    *   **Formel:** $ \text{Wertverlust} = RW_{alt,heute} - RW_{alt,in einem Jahr} $
2.  **Opportunitätskosten der Kapitalbindung (kalkulatorische Zinsen auf den heutigen Restwert):**
    *   Zinsen, die man alternativ erwirtschaften könnte, wenn man den heutigen Restwert (Liquidationserlös) anlegen würde.
    *   **Formel:** $ \text{Zinsen auf } RW_{alt,heute} = RW_{alt,heute} \times i $
3.  **Betriebskosten der alten Anlage für die nächste Periode:**
    *   Summe aus den fixen und variablen Betriebskosten, die im nächsten Jahr bei Weiterbetrieb anfallen.
    *   **Formel:** $ \text{Betriebskosten}_{alt,nächstes Jahr} = K_{fix,alt,nächstes Jahr} + (x \times k_{var,alt,nächstes Jahr}) $

**Gesamte Grenzkosten der alten Anlage für die nächste Periode:**
$$ GK_{alt,nächste Periode} = (\text{Wertverlust}) + (\text{Zinsen auf } RW_{alt,heute}) + (\text{Betriebskosten}_{alt,nächstes Jahr}) $$

#### **B. Berechnung der Durchschnittskosten der neuen Anlage pro Periode ($ØK_{neu}$)**

Diese werden berechnet wie in der normalen statischen Kostenvergleichsrechnung für die neue Anlage über deren *gesamte Nutzungsdauer*.

1.  **Durchschnittliche Abschreibung der neuen Anlage:**
    *   **Formel:** $ \text{Ø AfA}_{neu} = \frac{AW_{neu} - RW_{neu}}{ND_{neu}} $
2.  **Durchschnittlicher Kapitaleinsatz der neuen Anlage:**
    *   **Formel:** $ \text{Ø KE}_{neu} = \frac{AW_{neu} + RW_{neu}}{2} $
3.  **Durchschnittliche kalkulatorische Zinsen der neuen Anlage:**
    *   **Formel:** $ \text{Ø Zinsen}_{neu} = \text{Ø KE}_{neu} \times i $
4.  **Durchschnittliche jährliche Betriebskosten der neuen Anlage:**
    *   **Formel:** $ \text{Betriebskosten}_{neu,jährlich} = K_{fix,neu,jährlich} + (x \times k_{var,neu}) $
    *(Annahme: Die Produktionsmenge x ist für alt und neu vergleichbar oder es wird auf Stückkostenbasis verglichen)*

**Gesamte Durchschnittskosten der neuen Anlage pro Periode:**
$$ ØK_{neu} = \text{Ø AfA}_{neu} + \text{Ø Zinsen}_{neu} + \text{Betriebskosten}_{neu,jährlich} $$

**Stückkosten (falls Mengen unterschiedlich und Erlöse gleich):**
$ øk_{neu} = ØK_{neu} / x $
$ gk_{alt,nächste Periode} = GK_{alt,nächste Periode} / x $

#### **Beispielhafte Tabelle für den statischen Grenzkostenvergleich (für die Entscheidung "Weiterbetrieb 1 Jahr vs. Sofortiger Ersatz")**

| Kostenkomponente                                    | Alte Anlage (für nächstes Jahr) | Neue Anlage (Ø pro Jahr ihrer ND) |
| :-------------------------------------------------- | :------------------------------ | :-------------------------------- |
| **A. Grenzkosten alte Anlage (nächstes Jahr):**     |                                 |                                   |
| 1. Restwert (Liquidationserlös) heute ($RW_{alt,0}$)  | *gegeben*                       | -                                 |
| 2. Restwert (Liquidationserlös) in 1 Jahr ($RW_{alt,1}$) | *gegeben*                       | -                                 |
| 3. Wertverlust (Opportunitätskosten) ($RW_{alt,0} - RW_{alt,1}$) | **Berechnen**                   | -                                 |
| 4. Kalk. Zinsen auf $RW_{alt,0}$ ($RW_{alt,0} \times i$) | **Berechnen**                   | -                                 |
| 5. Fixe Betriebskosten nächstes Jahr                | *gegeben*                       | -                                 |
| 6. Variable Betriebskosten nächstes Jahr ($x \times k_{var,alt}$) | *gegeben/Berechnen*             | -                                 |
| **Summe Grenzkosten alte Anlage ($GK_{alt}$)**      | **Summe 3 bis 6**               | -                                 |
|                                                     |                                 |                                   |
| **B. Durchschnittskosten neue Anlage (pro Jahr):**  |                                 |                                   |
| 1. Anschaffungswert ($AW_{neu}$)                     | -                               | *gegeben*                         |
| 2. Restwert am Ende ND ($RW_{neu}$)                 | -                               | *gegeben*                         |
| 3. Nutzungsdauer ($ND_{neu}$)                       | -                               | *gegeben*                         |
| 4. Ø Abschreibung ($ (AW_{neu}-RW_{neu})/ND_{neu} $) | -                               | **Berechnen**                     |
| 5. Ø Kapitaleinsatz ($ (AW_{neu}+RW_{neu})/2 $)     | -                               | **Berechnen**                     |
| 6. Ø Kalk. Zinsen ($ ØKE_{neu} \times i $)          | -                               | **Berechnen**                     |
| 7. Fixe Betriebskosten p.a.                         | -                               | *gegeben*                         |
| 8. Variable Betriebskosten p.a. ($x \times k_{var,neu}$) | -                               | *gegeben/Berechnen*               |
| **Summe Durchschnittskosten neue Anlage ($ØK_{neu}$)**| -                               | **Summe 4, 6, 7, 8**              |
|                                                     |                                 |                                   |
| **Vergleichsbasis (z.B. Gesamt oder Stück):**       |                                 |                                   |
| Produktionsmenge (x)                                | *ggf. für Stückkosten*          | *ggf. für Stückkosten*            |
| **Grenzkosten/Stück alt ($GK_{alt}/x$)**            | *ggf. berechnen*                | -                                 |
| **Durchschnittskosten/Stück neu ($ØK_{neu}/x$)**     | -                               | *ggf. berechnen*                  |
| **Entscheidung:**                                   | *Wenn $GK_{alt} < ØK_{neu}$ => Weiterbetrieb* | *Wenn $ØK_{neu} < GK_{alt}$ => Ersatz* |
