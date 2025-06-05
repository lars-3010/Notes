---
tags:
  - 🌱
"up::":
  - "[[../../../Projects/Courses/_Investition und Finanzierung|_Investition und Finanzierung]]"
similar:
leads to:
  - "[[Break-Even-Analyse]]"
contradicts:
extends:
implements:
reviewed:
sources:
---
**Ziel:** Auswahl der Investitionsalternative mit dem höchsten (durchschnittlichen) Gewinn pro Periode.
**Anwendung:** Sinnvoll, wenn sich die Investitionsalternativen nicht nur in den Kosten, sondern auch in den Erlösen unterscheiden (z.B. durch unterschiedliche Produktqualität, unterschiedliche Absatzmengen zu unterschiedlichen Preisen).

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein:** Die Berechnung des Periodengewinns als Differenz von Erlösen und Kosten ist zentral. Die Fähigkeit, Erlöse korrekt zu ermitteln, kommt hinzu.
*   **Eher schlank behandeln (aber für Verständnis wichtig):** Die Break-Even-Analyse als spezifischer Punkt innerhalb der Gewinnbetrachtung.

#### **2.1. Ermittlung der Erlöse pro Periode**

*   **Name:** Gesamterlöse pro Periode (Eges)
*   **Formel:**
    $$ E_{ges} = \text{Absatzmenge (x)} \times \text{Verkaufspreis pro Stück (p)} $$
*   **Kurzerklärung:** Die gesamten Einnahmen, die durch den Verkauf der mit der Investition produzierten Güter/Dienstleistungen in der Durchschnittsperiode erzielt werden.

#### **2.2. Berechnung des Gewinns pro Periode**

*   **Name:** Gewinn pro Periode (G)
*   **Formel:**
    $$ G = E_{ges} - K_{ges} $$
    *Wobei:*
    *   $E_{ges}$ = Gesamterlöse pro Periode (siehe 2.1)
    *   $K_{ges}$ = Gesamtkosten pro Periode (berechnet wie in der Kostenvergleichsrechnung, siehe 1.2)
*   **Kurzerklärung:** Der Periodenerfolg der Investition.

**Entscheidungskriterium Gewinnvergleich:**
Wähle die Alternative mit dem **maximalen durchschnittlichen Gewinn** pro Periode.

**Tabellarisches Rechenschema für den Gewinnvergleich (Erweiterung des Kostenvergleichs-Schemas):**

| Position                          | Alternative A (€)                               | Alternative B (€)                               |
| :-------------------------------- | :---------------------------------------------- | :---------------------------------------------- |
| ... (Kosten wie im Kostenvergleich) | ...                                             | ...                                             |
| **3. Gesamtkosten p.a. (Kges)**   | **(Berechnet wie oben)**                        | **(Berechnet wie oben)**                        |
| **4. Erlöse p.a. (Eges):**        |                                                 |                                                 |
| Absatzmenge (x) p.a.              | *gegeben*                                       | *gegeben*                                       |
| Verkaufspreis/Stück (p)           | *gegeben*                                       | *gegeben*                                       |
| **Gesamterlöse p.a.**             | **x \* p**                                      | **x \* p**                                      |
| **5. Gewinn p.a. (G)**            | **Gesamterlöse p.a. - Gesamtkosten p.a.**     | **Gesamterlöse p.a. - Gesamtkosten p.a.**     |

#### **2.3. [[Break-Even-Analyse]] (Gewinnschwellenanalyse) – Schlanke Betrachtung**

**Ziel:** Ermittlung der Absatzmenge, bei der die Erlöse genau die Gesamtkosten decken (Gewinn = 0).
**Anwendung:** Hilft, das Risiko einer Investition einzuschätzen (wie viel muss mindestens verkauft werden?).

*   **Name:** Break-Even-Menge (MBEP) / Gewinnschwelle
*   **Grundidee:** Am Break-Even-Point gilt: Erlöse = Gesamtkosten
    $$ p \times m_{BEP} = (k_{var} \times m_{BEP}) + K_{fix,gesamt} $$
    *Wobei $K_{fix,gesamt}$ hier alle fixen Kostenkomponenten (inkl. Ø AfA und Ø Zinsen aus der statischen Betrachtung) umfasst.*
*   **Formel:**
    $$ m_{BEP} = \frac{K_{fix,gesamt}}{p - k_{var}} $$
    *Oder auch:*
    $$ m_{BEP} = \frac{K_{fix,gesamt}}{\text{Deckungsbeitrag pro Stück (db)}} $$
*   **Deckungsbeitrag pro Stück (db):**
    *   **Formel:** $db = p - k_{var}$
    *   **Kurzerklärung:** Der Betrag, der pro verkauftem Stück zur Deckung der Fixkosten und zur Gewinnerzielung beiträgt. *Für die Klausur reicht es meist, diesen als Teil der Break-Even-Formel zu verstehen, eine separate tiefergehende Deckungsbeitragsrechnung ist laut Fokus weniger wahrscheinlich.*
*   **Kurzerklärung zur Break-Even-Menge:** Die Absatzmenge, ab der die Investition beginnt, einen Gewinn zu erwirtschaften. Eine niedrige Gewinnschwelle ist tendenziell vorteilhafter (weniger Risiko).

**Wichtiger Hinweis für die Gewinnvergleichsrechnung und Break-Even-Analyse:**
Die hier verwendeten "Gesamtkosten" bzw. "Fixkosten gesamt" beinhalten die **kalkulatorischen Abschreibungen und kalkulatorischen Zinsen** aus der statischen Betrachtung, da diese für die Periodenbetrachtung der statischen Verfahren relevant sind.
