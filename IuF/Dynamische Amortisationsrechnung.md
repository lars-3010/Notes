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
**Ziel:** Ermittlung des Zeitraums, bis die ursprüngliche Anschaffungsauszahlung (I₀) durch die *Barwerte* der jährlichen Rückflüsse (Cashflows) der Investition gedeckt ist. Im Gegensatz zur statischen Amortisationsrechnung wird hier der Zeitwert des Geldes berücksichtigt.
**Anwendung:** Risikobeurteilung unter Berücksichtigung der Zinskosten für das gebundene Kapital. Eine kürzere dynamische Amortisationsdauer wird als weniger riskant angesehen.

**Vorüberlegung zum Fokus:**
*   **Zahlt auf den Fokus ein:** Das Verständnis, dass hier Barwerte kumuliert werden. Die Berechnung ist analog zur statischen Variante, nur eben mit abgezinsten Werten.

#### **5.1. Grundidee**

Die dynamische Amortisationsdauer ist der Zeitpunkt ($t_{A,dyn}$), zu dem der Kapitalwert der bis dahin angefallenen Zahlungen (inklusive der Anschaffungsauszahlung) gerade Null wird, wenn man nur die Zahlungen bis zu diesem Zeitpunkt $t_{A,dyn}$ betrachtet.
Oder anders ausgedrückt: Der Zeitpunkt, zu dem die Summe der Barwerte der laufenden Cashflows die Anschaffungsauszahlung erreicht.

#### **5.2. Berechnung der dynamischen Amortisationsdauer**

Das Vorgehen ist analog zur statischen Amortisationsrechnung bei unregelmäßigen Rückflüssen, nur dass anstelle der nominalen Cashflows deren Barwerte verwendet werden.

1.  **Berechne die Barwerte (BWt) der jährlichen Rückflüsse (CFt) für jede Periode t:**
    $$ BW_t = \frac{CF_t}{(1+i)^t} $$
    *Wobei `i` der Kalkulationszinssatz ist.*
2.  **Kumuliere die Barwerte der Rückflüsse Jahr für Jahr.**
3.  **Ermittle das Jahr, in dem die kumulierten Barwerte die Anschaffungsauszahlung (I₀) erstmals erreichen oder übersteigen.**
4.  **Interpolation für das letzte Jahr (falls die Deckung nicht genau am Jahresende erfolgt):**
    $$ \text{Anteil des letzten Jahres} = \frac{\text{Noch zu deckender Betrag (als Barwert) zu Beginn des letzten Jahres}}{\text{Barwert des Rückflusses im letzten Amortisationsjahr}} $$
    $$ t_{A,dyn} = (\text{Anzahl der vollen Jahre bis kurz vor Amortisation}) + \text{Anteil des letzten Jahres} $$

**Entscheidungskriterium Dynamische Amortisationsrechnung:**
Wähle die Alternative mit der **kürzesten dynamischen Amortisationsdauer**.
Eine Investition ist tendenziell vorteilhaft, wenn ihre dynamische Amortisationsdauer kürzer ist als ihre Nutzungsdauer (das bedeutet, der Kapitalwert wäre dann positiv).

**Tabellarisches Rechenschema für die dynamische Amortisationsdauer:**

| Jahr (t) | Zahlung / CFt (I₀, laufende CFs, RW) | Abzinsungsfaktor (AFt) bei Zinssatz i | Barwert (BWt = CFt \* AFt) | Kumulierter Barwert der Rückflüsse (Σ BWt ab t=1) |
| :------- | :------------------------------------ | :------------------------------------- | :------------------------- | :-------------------------------------------------------- |
| 0        | - I₀                                  | 1,0000                                 | - I₀                       |                                                           |
| 1        | CF₁                                   | $(1+i)^{-1}$                           | BW₁                        | BW₁                                                       |
| 2        | CF₂                                   | $(1+i)^{-2}$                           | BW₂                        | BW₁ + BW₂                                                 |
| ...      | ...                                   | ...                                    | ...                        | ...                                                       |
| $t_{A,dyn}^*$ | CF$_{t_{A,dyn}^*}$                   | $(1+i)^{-t_{A,dyn}^*}$                 | BW$_{t_{A,dyn}^*}$         | $\ge$ I₀                                                  |

*Wobei $t_{A,dyn}^*$ das Jahr ist, in dem die dynamische Amortisation erfolgt.*
*Beispiel für Interpolation (dynamisch):*
*I₀ = 1000. Bis Ende Jahr 2 sind kumulierte Barwerte von 800 erreicht. Der Barwert des Rückflusses im Jahr 3 sei 300.*
*Noch zu deckender Barwert: 1000 - 800 = 200.*
*Anteil Jahr 3: 200 / 300 = 0,67 Jahre.*
*Dynamische Amortisationsdauer: 2 Jahre + 0,67 Jahre = 2,67 Jahre.*

# Zusatz
---
**Ziel:** Zeitraum, bis I₀ durch die Barwerte der Rückflüsse gedeckt ist.  
**Vorgehen:** (Wie oben genannt) Kumulation der Barwerte der Rückflüsse.

**Beispielhafte Tabelle zur Berechnung der dynamischen Amortisationsdauer:**  
Anschaffungsauszahlung I₀ = 1000€, Kalkulationszinssatz i = 8%

|   |   |   |   |   |   |
|---|---|---|---|---|---|
|Jahr (t)|Rückfluss (CFt)|Abzinsungsfaktor (AFt) bei 8% (1,08)⁻ᵗ|Barwert (BWt = CFt * AFt)|Kumulierter Barwert der Rückflüsse|Noch zu decken (I₀ - Kum. BW)|
|0|-1000|1,0000|-1000||1000|
|1|300|0,9259|277,77|277,77|722,23|
|2|400|0,8573|342,92|620,69 (277,77+342,92)|379,31|
|3|500|0,7938|396,90|**1017,59** (620,69+396,90)|**-17,59** (Amortisation erfolgt)|
|4|200|0,7350|147,00|1164,59|-164,59|

Amortisation im 3. Jahr.  
Noch zu deckender Betrag zu Beginn des 3. Jahres: 379,31 €  
Barwert des Rückflusses im 3. Jahr: 396,90 €  
Anteil des 3. Jahres: $ \frac{379,31}{396,90} \approx 0,956 $ Jahre  
Dynamische Amortisationsdauer: $ 2 + 0,956 = 2,956 $ Jahre