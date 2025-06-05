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
>(Pay-Off-Periode / Payback-Periode)**

**Ziel:** Ermittlung des Zeitraums, der benötigt wird, bis die ursprüngliche Anschaffungsauszahlung (I₀) durch die jährlichen Rückflüsse (Cashflows) der Investition gedeckt ist. Es ist primär ein Maß für das Risiko einer Investition.
**Anwendung:** Schnellabschätzung des Risikos; je kürzer die Amortisationsdauer, desto schneller ist das investierte Kapital "wieder da" und desto geringer wird das Risiko eingeschätzt.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein:** Die Berechnung der Amortisationsdauer für konstante und unregelmäßige Rückflüsse. Das Verständnis, dass es hier um Liquidität und Risiko geht, weniger um Profitabilität.
*   **Wichtig:** Die statische Amortisationsrechnung arbeitet mit *nicht abgezinsten* Rückflüssen.

#### **4.1. Ermittlung des (durchschnittlichen) jährlichen Rückflusses (Cashflow vor Zinsen des Investors)**

Der Rückfluss ist das, was der Investition *liquide* wieder zufließt. Für die statische Amortisationsrechnung wird oft ein durchschnittlicher jährlicher Rückfluss verwendet.

*   **Name:** (Durchschnittlicher) Jährlicher Rückfluss / Cashflow (CF)
*   **Formel:**
    $$ \text{Jährlicher Rückfluss (CF)} = \text{Gewinn nach Steuern (falls relevant, sonst Gewinn)} + \text{Abschreibungen} $$
    *Erläuterung der Komponenten:*
    *   **Gewinn:** Typischerweise wird hier der *Gewinn nach Zinskosten für Fremdkapital (falls vorhanden und explizit gegeben), aber vor kalkulatorischen Zinsen des Investors* verwendet. Wenn keine expliziten Fremdkapitalzinsen gegeben sind, nimmt man oft den Gewinn nach Abschreibungen (also $E_{ges} - K_{betrieblich,fix} - K_{var} - AfA$).
    *   **Abschreibungen (Ø AfA):** Da Abschreibungen zwar den Gewinn mindern, aber keine tatsächliche Auszahlung in der Periode darstellen (die Auszahlung erfolgte ja bei der Anschaffung), werden sie zum Gewinn hinzuaddiert, um den liquiden Mittelzufluss zu erhalten.
*   **Alternative Berechnung des Rückflusses (wenn Erlöse und auszahlungswirksame Kosten gegeben sind):**
    $$ \text{Jährlicher Rückfluss (CF)} = \text{Erlöse} - (\text{auszahlungswirksame fixe Kosten} + \text{auszahlungswirksame variable Kosten}) $$
    *Diese Betrachtung ist direkter auf die Liquidität bezogen.*
*   **Kurzerklärung:** Der jährliche Betrag an liquiden Mitteln, der aus der Investition zurückfließt und zur Deckung der ursprünglichen Anschaffungsauszahlung zur Verfügung steht.

**Wichtiger Hinweis für Klausuren:** Oft wird der Einfachheit halber der "Gewinn" aus der Gewinnvergleichsrechnung (der die kalkulatorischen Zinsen bereits als Kosten enthält) plus die Abschreibungen als Rückfluss genommen. Achte genau auf die Aufgabenstellung, welcher "Gewinn" gemeint ist. Die konzeptionell sauberste Definition für den Rückfluss zur Amortisation ist der *Einzahlungsüberschuss vor Zinsen und Steuern des Gesamtprojekts* (EBITDA) oder zumindest *vor Zinsen des Investors*. Da hier aber oft mit dem statischen "Gewinnbegriff" gearbeitet wird, ist "Gewinn + AfA" eine häufige Vereinfachung.

#### **4.2. Berechnung der Amortisationsdauer**

*   **Fall 1: Konstante jährliche Rückflüsse (CF):**
    *   **Name:** Statische Amortisationsdauer ($t_A$)
    *   **Formel:**
        $$ t_A = \frac{\text{Anschaffungsauszahlung (I}_0\text{)}}{\text{Jährlicher Rückfluss (CF)}} $$
    *   **Kurzerklärung:** Wenn jedes Jahr der gleiche Betrag zurückfließt, ist die Berechnung einfach.

*   **Fall 2: Unregelmäßige jährliche Rückflüsse:**
    *   **Name:** Statische Amortisationsdauer ($t_A$)
    *   **Vorgehen (Kumulation):**
        1.  Liste die jährlichen Rückflüsse auf.
        2.  Kumuliere die Rückflüsse Jahr für Jahr.
        3.  Ermittle das Jahr, in dem die kumulierten Rückflüsse die Anschaffungsauszahlung (I₀) erstmals erreichen oder übersteigen.
        4.  **Interpolation für das letzte Jahr (falls die Deckung nicht genau am Jahresende erfolgt):**
            $$ \text{Anteil des letzten Jahres} = \frac{\text{Noch zu deckender Betrag zu Beginn des letzten Jahres}}{\text{Rückfluss im letzten Amortisationsjahr}} $$
            $$ t_A = (\text{Anzahl der vollen Jahre bis kurz vor Amortisation}) + \text{Anteil des letzten Jahres} $$
    *   **Kurzerklärung:** Man zählt, wie viele Jahre es dauert, bis I₀ "zurückverdient" ist.

**Entscheidungskriterium Amortisationsrechnung:**
Wähle die Alternative mit der **kürzesten Amortisationsdauer**. Es gibt oft eine vom Unternehmen vorgegebene maximale Amortisationsdauer.

**Tabellarisches Rechenschema für Amortisationsdauer bei unregelmäßigen Rückflüssen:**

| Jahr (t) | Jährlicher Rückfluss (CFt) | Kumulierter Rückfluss (Σ CFt) | Noch zu deckender Betrag (I₀ - Σ CFt) |
| :------- | :------------------------- | :--------------------------- | :------------------------------------- |
| 0        | - I₀                       | - I₀                         | I₀                                     |
| 1        | CF₁                        | CF₁ - I₀                     | I₀ - CF₁                               |
| 2        | CF₂                        | CF₁ + CF₂ - I₀               | I₀ - (CF₁ + CF₂)                       |
| ...      | ...                        | ...                          | ...                                    |
| $t_A^*$  | CF$_{t_A^*}$               | $\ge$ I₀                     | $\le$ 0                                |

*Wobei $t_A^*$ das Jahr ist, in dem die Amortisation erfolgt.*
*Beispiel für Interpolation:*
*I₀ = 1000. Bis Ende Jahr 2 sind 800 kumuliert. Im Jahr 3 ist der Rückfluss 300.*
*Noch zu decken: 1000 - 800 = 200.*
*Anteil Jahr 3: 200 / 300 = 0,67 Jahre.*
*Amortisationsdauer: 2 Jahre + 0,67 Jahre = 2,67 Jahre.*
