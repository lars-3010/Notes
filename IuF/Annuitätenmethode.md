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
**Ziel:** Umrechnung des Kapitalwerts (KW) einer Investition in eine gleichbleibende jährliche Zahlung (Annuität, AN) über die gesamte Nutzungsdauer der Investition. Diese Annuität repräsentiert den durchschnittlichen jährlichen Überschuss, den die Investition über die Deckung der Kapitalkosten (Abschreibung und Verzinsung des gebundenen Kapitals zum Kalkulationszinssatz) hinaus erwirtschaftet.
**Anwendung:** Besonders nützlich für den Vergleich von Investitionen mit unterschiedlicher Nutzungsdauer, da sie den Erfolg auf eine einheitliche Periodengröße (jährlicher Betrag) herunterbricht.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein:** Das Verständnis, wie die Annuität aus dem Kapitalwert abgeleitet wird, die Berechnung mittels Kapitalwiedergewinnungsfaktor (oder dessen Kehrwert, dem Rentenbarwertfaktor) und die Entscheidungsregel.
*   **Wichtig für Verständnis:** Die Annuität ist quasi der "verjährlichte" Kapitalwert.

#### **4.1. Formeln**

*   **Name:** Annuität (AN)
*   **Grundidee:** Die Annuität ist der Betrag, der periodisch (z.B. jährlich) entnommen werden kann, sodass am Ende der Laufzeit das ursprünglich investierte Kapital (inklusive Verzinsung zum Kalkulationszinssatz i) getilgt ist und der Kapitalwert (als zusätzlicher Vermögenszuwachs) ebenfalls in gleichmäßigen Raten über die Laufzeit verteilt wird.
*   **Formel (unter Verwendung des Kapitalwiedergewinnungsfaktors KWF, auch Annuitätenfaktor ANF genannt):**
    $$ AN = KW \times KWF(i, n) $$
    *Oder, was identisch ist, unter Verwendung des Rentenbarwertfaktors RBF (da KWF = 1/RBF):*
    $$ AN = \frac{KW}{RBF(i, n)} $$

*   **Kapitalwiedergewinnungsfaktor (KWF) / Annuitätenfaktor (ANF):**
    *   **Name:** Kapitalwiedergewinnungsfaktor (KWF) oder Annuitätenfaktor (ANF)
    *   **Formel:**
        $$ KWF(i, n) = ANF(i, n) = \frac{i \times (1+i)^n}{(1+i)^n - 1} $$
    *   **Kurzerklärung:** Dieser Faktor wandelt einen heutigen Barwert (den KW) in eine Serie von gleich hohen zukünftigen Zahlungen (die Annuität) um. Er ist der Kehrwert des Rentenbarwertfaktors. *In Klausuren sind oft Tabellen für KWF/ANF oder RBF gegeben.*

*   **Rentenbarwertfaktor (RBF):**
    *   **Name:** Rentenbarwertfaktor (RBF)
    *   **Formel:**
        $$ RBF(i, n) = \frac{(1+i)^n - 1}{i \times (1+i)^n} $$
    *   **Kurzerklärung:** Dieser Faktor wandelt eine Serie von gleich hohen zukünftigen Zahlungen (eine Rente/Annuität) in einen heutigen Barwert um.

    *Wobei für alle Formeln gilt:*
    *   `KW` = Kapitalwert der Investition
    *   `i` = Kalkulationszinssatz pro Periode (als Dezimalzahl)
    *   `n` = Nutzungsdauer der Investition

*   **Kurzerklärung zur Annuität:** Der jährliche, konstante Betrag, den die Investition über ihre gesamte Nutzungsdauer "abwirft", nachdem alle Kosten (inkl. kalkulatorischer Verzinsung des gebundenen Kapitals) gedeckt sind und die Anschaffungsauszahlung getilgt wurde. Sie ist direkt aus dem Kapitalwert abgeleitet.

#### **4.2. Entscheidungsregel**

*   **Einzelinvestition:** Eine Investition ist vorteilhaft, wenn ihre **Annuität (AN) > 0** ist.
    *   AN > 0: Die Investition erwirtschaftet durchschnittlich pro Jahr mehr als die geforderte Mindestverzinsung und die Tilgung. (Entspricht KW > 0)
    *   AN = 0: Die Investition erwirtschaftet durchschnittlich pro Jahr genau die geforderte Mindestverzinsung und die Tilgung. (Entspricht KW = 0)
    *   AN < 0: Die Investition erwirtschaftet durchschnittlich pro Jahr weniger als die geforderte Mindestverzinsung und die Tilgung. (Entspricht KW < 0)
*   **Auswahl zwischen mehreren Alternativen:** Wähle die Alternative mit der **höchsten positiven Annuität**. Dies ist besonders sinnvoll, wenn die Alternativen unterschiedliche Nutzungsdauern haben.

#### **4.3. Berechnungsschritte**

1.  **Kapitalwert (KW) berechnen:** Verwende die Kapitalwertmethode (siehe Abschnitt 2 dieses Blocks).
2.  **Kapitalwiedergewinnungsfaktor (KWF) ermitteln:**
    *   Entweder aus einer Formelsammlung/Tabelle ablesen (für gegebenes i und n).
    *   Oder berechnen mit der Formel: $ KWF(i, n) = \frac{i \times (1+i)^n}{(1+i)^n - 1} $
    *   Alternativ: Rentenbarwertfaktor (RBF) ermitteln und dann $KWF = 1/RBF$.
3.  **Annuität (AN) berechnen:** $AN = KW \times KWF$.

**Beispielhafter Rechenweg (ohne Tabelle für KWF, Berechnung über RBF):**

*Gegeben: KW = 1000€, i = 8% (0,08), n = 5 Jahre*

1.  Berechne RBF(8%, 5 Jahre):
    $ RBF = \frac{(1+0,08)^5 - 1}{0,08 \times (1+0,08)^5} = \frac{(1,08)^5 - 1}{0,08 \times (1,08)^5} = \frac{1,469328 - 1}{0,08 \times 1,469328} = \frac{0,469328}{0,117546} \approx 3,9927 $
2.  Berechne Annuität:
    $ AN = \frac{KW}{RBF} = \frac{1000€}{3,9927} \approx 250,46€ $

Das bedeutet, die Investition mit einem KW von 1000€ erwirtschaftet über 5 Jahre bei 8% Kalkulationszins einen durchschnittlichen jährlichen Überschuss von ca. 250,46€.



# Zusatz

**Ziel:** Umrechnung des Kapitalwerts (KW) in eine gleichbleibende jährliche Zahlung (Annuität, AN) über die Nutzungsdauer.
**Formeln:** (Bereits in vorheriger Antwort genannt)
*   $ AN = KW \times KWF(i, n) $ oder $ AN = \frac{KW}{RBF(i, n)} $
*   $ KWF(i, n) = \frac{i \times (1+i)^n}{(1+i)^n - 1} $ (Kapitalwiedergewinnungsfaktor)
*   $ RBF(i, n) = \frac{(1+i)^n - 1}{i \times (1+i)^n} $ (Rentenbarwertfaktor)

**Zahlungsreihe und Annuität – Konzeptionelles Verständnis:**
Stell dir vor, eine Investition hat einen Kapitalwert von z.B. 1000 € bei einer Nutzungsdauer von 3 Jahren und einem Kalkulationszinssatz von 10%. Die Annuität beantwortet die Frage: Welchen *gleichbleibenden jährlichen Betrag* kann ich über diese 3 Jahre aus der Investition entnehmen, sodass der heutige Wert dieser Entnahmen genau dem Kapitalwert von 1000 € entspricht?

**Beispielhafte Darstellung (konzeptionell):**
*Investition I₀ führt zu Zahlungsreihe CF₁, CF₂, CF₃.*
*Daraus ergibt sich KW.*
*Die Annuitätenmethode transformiert dies in eine äquivalente Zahlungsreihe: AN, AN, AN.*

| Jahr (t) | Ursprüngliche Zahlungsreihe (Beispiel) | Barwert der Zahlung | Äquivalente Annuitätenreihe |
| :------- | :------------------------------------- | :------------------ | :--------------------------- |
| 0        | -5000 (I₀)                             | -5000               |                              |
| 1        | +2000 (CF₁)                            | +1818 (bei i=10%)   | +AN                          |
| 2        | +2500 (CF₂)                            | +2066 (bei i=10%)   | +AN                          |
| 3        | +3000 (CF₃)                            | +2254 (bei i=10%)   | +AN                          |
| **KW**   |                                        | **+1138**           |                              |

*Berechnung der Annuität:*
$RBF(10\%, 3 J.) = \frac{(1,10)^3 - 1}{0,10 \times (1,10)^3} \approx 2,48685$
$AN = \frac{1138 €}{2,48685} \approx 457,61 €$

Das bedeutet, die Investition ist gleichwertig zu einer jährlichen Zahlung von 457,61 € über 3 Jahre, zusätzlich zur Deckung der ursprünglichen Investition und deren Verzinsung mit 10%.

**Entscheidungsregel:** (Wie oben genannt)
*   Einzelinvestition: Vorteilhaft, wenn $AN > 0$.
*   Auswahl: Höchste positive Annuität (besonders bei unterschiedlichen Nutzungsdauern).
