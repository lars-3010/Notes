---
tags:
  - 🌱
"up::":
  - "[[Gewinnvergleichsrechnung]]"
similar:
leads to:
contradicts:
extends:
implements:
reviewed:
sources:
---
**1. Grundkonzept und Ziel:**

*   **Was ist der Break-Even-Point (BEP)?**
    *   Der BEP ist die Produktions- und Absatzmenge (oder der Umsatz), bei der die **Gesamterlöse genau den Gesamtkosten entsprechen**.
    *   An diesem Punkt macht das Unternehmen **weder Gewinn noch Verlust** (Gewinn = 0).
    *   Er wird auch als **Gewinnschwelle** oder **Nutzenschwelle** bezeichnet.
*   **Warum ist er wichtig?**
    *   **Risikobeurteilung:** Er zeigt, wie viel mindestens produziert und verkauft werden muss, um alle Kosten zu decken. Eine niedrige Gewinnschwelle bedeutet ein geringeres Risiko, da schneller Gewinne erzielt werden.
    *   **Preis- und Produktentscheidungen:** Hilft bei der Kalkulation von Mindestpreisen oder bei der Entscheidung, ob ein Produkt überhaupt angeboten werden soll.
    *   **Kapazitätsplanung:** Gibt Hinweise auf die notwendige Auslastung.

**2. Komponenten und Annahmen:**

*   **Fixkosten ($K_{fix}$):** Kosten, die unabhängig von der Produktionsmenge anfallen (z.B. Miete, Gehälter, Abschreibungen, kalkulatorische Zinsen im statischen Kontext).
*   **Variable Kosten ($k_{var}$ pro Stück):** Kosten, die direkt mit jeder produzierten Einheit anfallen (z.B. Materialkosten, Akkordlöhne).
*   **Verkaufspreis ($p$ pro Stück):** Der Preis, zu dem eine Einheit verkauft wird.
*   **Lineare Kosten- und Erlösverläufe:** Die klassische Break-Even-Analyse geht davon aus, dass Fixkosten konstant sind, variable Kosten pro Stück konstant sind und der Verkaufspreis pro Stück konstant ist. Das führt zu linearen Funktionen für Gesamtkosten und Gesamterlöse.
*   **Produktionsmenge = Absatzmenge:** Es wird unterstellt, dass alles, was produziert wird, auch verkauft wird (keine Lagerbestandsveränderungen).

**3. Berechnung des Break-Even-Points:**

*   **Grundgleichung am BEP:**
    $$ \text{Gesamterlöse (E)} = \text{Gesamtkosten (K)} $$
    $$ p \times m_{BEP} = (k_{var} \times m_{BEP}) + K_{fix} $$
    *Wobei $m_{BEP}$ die Break-Even-Menge ist.*

*   **Herleitung der Formel für die Break-Even-Menge:**
    1.  $p \times m_{BEP} - k_{var} \times m_{BEP} = K_{fix}$
    2.  $m_{BEP} \times (p - k_{var}) = K_{fix}$
    3.  $$ m_{BEP} = \frac{K_{fix}}{p - k_{var}} $$

*   **Deckungsbeitrag (DB):**
    *   **Definition:** Der Deckungsbeitrag ist die Differenz zwischen dem Erlös und den variablen Kosten. Er gibt an, wie viel ein Produkt oder eine Leistungseinheit zur Deckung der Fixkosten und zur Gewinnerzielung beiträgt.
    *   **Deckungsbeitrag pro Stück ($db_{Stück}$):**
        $$ db_{Stück} = p - k_{var} $$
    *   **Gesamter Deckungsbeitrag ($DB_{Gesamt}$):**
        $$ DB_{Gesamt} = \text{Gesamterlöse} - \text{Gesamte variable Kosten} = m \times (p - k_{var}) = m \times db_{Stück} $$
    *   **Bedeutung am BEP:** Am Break-Even-Point ist der gesamte Deckungsbeitrag genau so hoch wie die Fixkosten: $DB_{Gesamt, BEP} = K_{fix}$.
    *   **BEP-Formel mit Deckungsbeitrag:**
        $$ m_{BEP} = \frac{K_{fix}}{db_{Stück}} $$

*   **Break-Even-Umsatz ($U_{BEP}$):**
    *   Manchmal ist es auch interessant zu wissen, welcher Umsatz erzielt werden muss, um die Gewinnschwelle zu erreichen.
    *   **Formel:**
        $$ U_{BEP} = m_{BEP} \times p $$
    *   Oder über den Deckungsbeitragssatz (DB-Satz = $db_{Stück} / p$ oder $DB_{Gesamt} / U_{Gesamt}$):
        $$ U_{BEP} = \frac{K_{fix}}{\text{DB-Satz}} $$

**4. Grafische Darstellung (Folie 21):**

*   Auf der X-Achse wird die Menge (m) abgetragen, auf der Y-Achse Kosten und Erlöse (€).
*   **Fixkostenkurve:** Eine horizontale Linie auf Höhe der Fixkosten.
*   **Gesamtkostenkurve:** Beginnt bei den Fixkosten (bei Menge 0) und steigt linear mit der Steigung der variablen Stückkosten ($k_{var}$).
    *   $K(m) = K_{fix} + k_{var} \times m$
*   **Gesamterlöskurve:** Beginnt im Ursprung (bei Menge 0) und steigt linear mit der Steigung des Verkaufspreises ($p$).
    *   $E(m) = p \times m$
*   **Break-Even-Point:** Der Schnittpunkt der Gesamtkostenkurve und der Gesamterlöskurve.
    *   Links vom BEP: Verlustzone (Kosten > Erlöse).
    *   Rechts vom BEP: Gewinnzone (Erlöse > Kosten).

**5. Angrenzende Themen und Erweiterungen (eher für tiefergehendes Verständnis, nicht unbedingt Klausurfokus):**

*   **Sicherheitskoeffizient / Sicherheitsmarge:**
    *   Gibt an, um wie viel Prozent die aktuelle Absatzmenge (oder der Umsatz) über der Break-Even-Menge (oder dem Break-Even-Umsatz) liegt.
    *   Formel (mengenbasiert): $\text{Sicherheitsmarge} = \frac{\text{Ist-Menge} - m_{BEP}}{\text{Ist-Menge}} \times 100\%$
    *   Ein Maß für das Risiko: Je höher die Sicherheitsmarge, desto weiter kann der Absatz zurückgehen, bevor Verluste entstehen. (Deine Folie 24 erwähnt den Sicherheitskoeffizienten).
*   **Deckungsbeitragsrechnung:**
    *   Der Deckungsbeitrag ist ein zentrales Konzept im internen Rechnungswesen (Kostenrechnung) für Produkt-, Preis- und Programmentscheidungen (z.B. Ermittlung von Preisuntergrenzen, Entscheidung über Annahme von Zusatzaufträgen, Optimierung des Produktionsprogramms bei Engpässen).
    *   Für die *statische Investitionsrechnung* ist er primär im Kontext des BEP relevant.
*   **Mehrprodukt-Break-Even-Analyse:**
    *   Wenn ein Unternehmen mehrere Produkte herstellt, wird die BEP-Analyse komplexer, da die Fixkosten auf die Produkte aufgeteilt oder ein durchschnittlicher Deckungsbeitrag (gewichtet mit dem Absatzmix) verwendet werden muss. (Wahrscheinlich nicht Klausurfokus).
*   **Nichtlineare Kosten- und Erlösverläufe:**
    *   In der Realität sind Kosten- und Erlösfunktionen nicht immer linear (z.B. Mengenrabatte beim Einkauf, degressive Preise bei hohen Absatzmengen). Dies führt zu komplexeren BEP-Analysen mit ggf. mehreren Gewinnschwellen. (Definitiv nicht Klausurfokus).

**Zusammenfassend für die Klausur:**

*   **Verstehe das Ziel und die Aussage des BEP.**
*   **Kenne die Formel zur Berechnung der Break-Even-Menge ($m_{BEP} = K_{fix} / (p - k_{var})$) und wisse, dass $(p - k_{var})$ der Deckungsbeitrag pro Stück ist.**
*   Sei in der Lage, die **Fixkosten ($K_{fix}$)** für die BEP-Berechnung im Kontext einer statischen Investitionsrechnung korrekt zu ermitteln (dazu gehören i.d.R. betriebliche Fixkosten + Ø Abschreibungen + Ø kalkulatorische Zinsen).
*   Du solltest die **grafische Darstellung interpretieren** können.