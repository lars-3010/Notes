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
**Ziel:** Bestimmung des Zeitraums, über den eine Investition betrieben werden sollte, um ihren Wertbeitrag (gemessen am Kapitalwert oder der Annuität) zu maximieren.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein (A-Priorität Folie 62, aber Rechenbeispiele 63-64 als C markiert):** Das *Konzept* der optimalen Nutzungsdauer und die Logik sind wichtig. Die detaillierte Berechnung für unendlichen Horizont ist komplex und laut deiner C-Priorisierung weniger wahrscheinlich für eine tiefe Rechenaufgabe. Die einmalige Investition ist das Grundverständnis.
*   Wir konzentrieren uns auf das Prinzip der einmaligen Investition und erwähnen den unendlichen Horizont konzeptionell mit der Annuitätenlogik.

#### **1.1. Optimale Nutzungsdauer bei einmaliger Investition (Single Investment Horizon)**

**Vorgehen:**

1.  **Definiere mögliche Nutzungsdauern (n):** Von n=1 Jahr bis zur maximal technisch/wirtschaftlich sinnvollen Dauer (N_max).
2.  **Erstelle für jede mögliche Nutzungsdauer (n) eine eigene Zahlungsreihe:**
    *   Anschaffungsauszahlung I₀ (bleibt gleich).
    *   Laufende Cashflows (CFt) von t=1 bis zur jeweiligen betrachteten Nutzungsdauer n.
    *   **Wichtig:** Der Restwert (RWn) am Ende der *jeweiligen* Nutzungsdauer n muss berücksichtigt werden. Der Restwert wird in der Regel sinken, je länger die Nutzungsdauer ist.
3.  **Berechne für jede dieser Zahlungsreihen den Kapitalwert KW(n)** mit dem gegebenen Kalkulationszinssatz i.
4.  **Entscheidung:** Wähle die Nutzungsdauer $n^*$, für die der Kapitalwert $KW(n^*)$ maximal wird.

**Beispielhafte Tabelle zur Ermittlung der optimalen Nutzungsdauer (Einmalige Investition):**
*Kalkulationszinssatz i = 10%*

| Mögliche Nutzungsdauer (n) | I₀    | CF₁ | RW₁ | CF₂ | RW₂ | CF₃ | RW₃ | ... | **KW(n)** bei i=10% |
| :------------------------- | :---- | :-- | :-- | :-- | :-- | :-- | :-- | :-- | :------------------ |
| **1 Jahr**                 | -1000 | 600 | 500 |     |     |     |     |     | $KW(1) = \frac{600+500}{1,10} - 1000 = 0$ |
| **2 Jahre**                | -1000 | 600 |     | 400 | 300 |     |     |     | $KW(2) = \frac{600}{1,10} + \frac{400+300}{(1,10)^2} - 1000 = \approx +24,79$ |
| **3 Jahre**                | -1000 | 600 |     | 400 |     | 200 | 100 |     | $KW(3) = \frac{600}{1,10} + \frac{400}{(1,10)^2} + \frac{200+100}{(1,10)^3} - 1000 = \approx +103,83$ **(Optimum in diesem Bsp.)** |
| **4 Jahre**                | -1000 | 600 |     | 400 |     | 200 |     | ... | $KW(4) = ... \text{ (könnte wieder sinken)}$ |

*Anmerkung: In der Tabelle oben sind CF und RW kombiniert im letzten Jahr der jeweiligen Nutzungsdauer.*
*Die Logik deiner Folie 64 ist genau diese: Es werden für jede potenzielle Nutzungsdauer (Zeilen 0 bis 6) die entsprechenden Cashflows der jeweiligen Jahre (Spalten 0 bis 6, wobei die Zahl in der Zelle der Cashflow des Jahres *Spalte* ist, wenn die Nutzungsdauer die der *Zeile* ist) und der Restwert am Ende dieser Nutzungsdauer verwendet, um den KW zu berechnen. Die Zeile mit dem höchsten KW gibt die optimale Nutzungsdauer an.*

**Formel (Ziel):**
$$ \max_{n} KW(n) = \max_{n} \left( \sum_{t=1}^{n} \frac{CF_t}{(1+i)^t} + \frac{RW_n}{(1+i)^n} - I_0 \right) $$

#### **1.2. Optimale Nutzungsdauer bei mehrmaliger identischer Investition (Unendlicher Planungshorizont / Replacement Chain) – Konzeptionell**

**Grundidee (Folie 65, 67):** Wenn eine Investition durch eine identische Folgeinvestition ersetzt wird (und das unendlich oft), sucht man die Nutzungsdauer, die den höchsten *durchschnittlichen jährlichen Wertbeitrag* über unendliche Zeit liefert. Dies wird erreicht, indem man die Nutzungsdauer wählt, welche die **höchste Annuität (AN)** für einen einzelnen Investitionszyklus generiert. Der Gesamtkapitalwert (GKW) einer unendlichen Kette dieser Annuitäten ist dann $AN/i$.

**Vorgehen (konzeptionell):**

1.  Berechne für jede mögliche Nutzungsdauer n eines einzelnen Investitionszyklus den Kapitalwert KW(n) (wie bei der einmaligen Investition).
2.  Wandle jeden KW(n) in die dazugehörige Annuität AN(n) um: $AN(n) = KW(n) \times KWF(i,n)$.
3.  Wähle die Nutzungsdauer $n^*$, für die $AN(n^*)$ maximal wird.
4.  (Optional: Der Gesamtkapitalwert der unendlichen Kette ist dann $GKW = AN(n^*) / i$).

**Formel (Ziel für unendlichen Horizont):**
$$ \max_{n} AN(n) \quad \text{oder äquivalent} \quad \max_{n} \frac{KW(n) \cdot KWF(i,n)}{i} = \max_{n} \frac{AN(n)}{i} $$
Dein Folienbeispiel 68 zeigt genau das: Es wird der KW für verschiedene Nutzungsdauern berechnet, dann die Annuität (mittels AF = KWF) und schließlich der GKW (Annuität / Zins). Die höchste Annuität (und damit der höchste GKW) bestimmt die optimale Nutzungsdauer.

**Für die Klausur (Fokus):**
*   Das Prinzip der KW-Maximierung für die **einmalige Investition** sicher beherrschen (Tabelle wie auf Folie 64).
*   Für den **unendlichen Horizont** das Konzept verstehen, dass über die Maximierung der Annuität die optimale Kettungsdauer gefunden wird. Die detaillierte GKW-Formel ist gut zu wissen, aber die Kernlogik ist die Annuitätenmaximierung.
