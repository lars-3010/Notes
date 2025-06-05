---
tags:
  - 🌱
"up::":
  - "[[../../../../Projects/Courses/_Investition und Finanzierung|_Investition und Finanzierung]]"
  - "[[Formelsammlung - dynamische Investitionsverfahren]]"
similar:
leads to:
  - "[[Formelsammlung - Finanzierung & Kennzahlen]]"
contradicts:
extends:
implements:
reviewed:
sources:
---
**Grundgedanke:** Anwendung der dynamischen Verfahren zur Lösung spezifischer Entscheidungsprobleme über Zeiträume oder bei Ressourcenknappheit.

---

**1. Optimale Nutzungsdauer (ND_opt)**

*Entscheidungskriterium: Wähle die Nutzungsdauer, die den relevanten Wertbeitrag (KW bei einmaliger Investition, Annuität bei unendlicher Kette) maximiert.*

**1.1. Einmalige Investition**
*   **Zweck:** Bestimmung der Laufzeit, die den Kapitalwert einer einzelnen, nicht wiederholten Investition maximiert.
*   **Vorgehen:**
    1.  Für jede mögliche Nutzungsdauer `n` (von 1 bis $N_{max}$):
        *   Definiere die Zahlungsreihe: $-I_0, CF_1, ..., CF_n + RW_n$ (Restwert $RW_n$ ist abhängig von der gewählten Nutzungsdauer n).
        *   Berechne den Kapitalwert $KW(n)$ dieser Zahlungsreihe.
    2.  Wähle die Nutzungsdauer $n^*$, für die $KW(n^*)$ maximal ist.
*   **Tabellarisches Schema zur Lösungsfindung:**

    | Mögliche ND (n) | $CF_0$ | $CF_1$ | $RW_1$ | $CF_2$ | $RW_2$ | ... | $CF_n+RW_n$ | **KW(n)** bei i |
    | :-------------- | :----- | :----- | :----- | :----- | :----- | :-- | :---------- | :-------------- |
    | 1 Jahr          | -$I_0$ | $CF_1$ | $RW_1$ |        |        |     |             | $KW(1)$         |
    | 2 Jahre         | -$I_0$ | $CF_1$ |        | $CF_2$ | $RW_2$ |     |             | $KW(2)$         |
    | ...             | -$I_0$ | ...    |        | ...    |        | ... | $CF_n+RW_n$ | $KW(n)$         |
    | $N_{max}$       | -$I_0$ | ...    |        | ...    |        |     | $CF_{Nmax}+RW_{Nmax}$ | $KW(N_{max})$   |
    *(Hinweis: $CF_t$ sind die laufenden Cashflows, $RW_n$ der Restwert am Ende der jeweiligen Nutzungsdauer n).*

**1.2. *Konzept:* Mehrmalige identische Investition (Unendlicher Planungshorizont)**
*   **Zweck:** Bestimmung der optimalen Zyklusdauer für eine Investition, die unendlich oft durch eine identische ersetzt wird.
*   **Vorgehen:**
    1.  Berechne für jede mögliche Nutzungsdauer `n` eines einzelnen Zyklus den $KW(n)$ (wie oben).
    2.  Wandle jeden $KW(n)$ in die zugehörige Annuität $AN(n)$ um: $AN(n) = KW(n) \times KWF(i,n)$.
    3.  Wähle die Nutzungsdauer $n^*$, für die $AN(n^*)$ maximal ist.
    *   *(Der Gesamtkapitalwert der unendlichen Kette ist dann $GKW = AN(n^*) / i$).*
*   **Tabellarisches Schema zur Lösungsfindung (Erweiterung von oben):**

    | Mögliche ND (n) | $KW(n)$ (aus 1.1) | $KWF(i,n)$ (oder RBF) | $AN(n) = KW(n) \times KWF(i,n)$ | $GKW = AN(n)/i$ (Optional) |
    | :-------------- | :---------------- | :-------------------- | :------------------------------ | :-------------------------- |
    | 1 Jahr          | $KW(1)$           | ...                   | $AN(1)$                         | $GKW(1)$                    |
    | 2 Jahre         | $KW(2)$           | ...                   | $AN(2)$                         | $GKW(2)$                    |
    | ...             | ...               | ...                   | ...                             | ...                         |
    *(Entscheidung für n mit max. AN(n) oder max. GKW)*

---

**2. Optimaler Ersatzzeitpunkt (Dynamisch mit KW-Vergleich der Strategien)**

*Entscheidungskriterium: Wähle die Ersatzstrategie mit dem **höchsten Gesamtkapitalwert**.*

**2.1. Grundidee:** Vergleiche den Kapitalwert verschiedener Strategien, die definieren, wann eine alte Anlage durch eine neue ersetzt wird.
**Wichtige Elemente (pro Strategie $S_k$: Ersatz nach k Jahren):**
*   **Opportunitätskosten in t=0 (bei k>0):** $-RW_{alt,0}$ (Verzicht auf sofortigen Verkauf).
*   **Erlös in t=0 (bei k=0):** $+RW_{alt,0}$ (Sofortiger Verkauf).
*   **Zahlungen der alten Anlage:** $CF_{alt,t}$ für t=1 bis k, und $+RW_{alt,k}$ im Jahr k.
*   **Wert der neuen Anlage ab Ersatz:** Entweder $KW_{neu}$ (wenn als einmalige Investition) oder eine Annuitätenkette $AN_{neu}$ (wenn als unendlicher Ersatz oder für einen definierten Folgezeitraum). Der Barwert dieses Teils muss auf t=0 diskontiert werden, beginnend ab dem Ersatzzeitpunkt k.

**2.2. Schema für Kapitalwert einer Strategie $S_k$ (Ersatz nach k Jahren, neue Anlage als $KW_{neu}$):**
$$ KW_{Sk} = \underbrace{\left( \sum_{t=1}^{k} \frac{CF_{alt,t}}{(1+i)^t} + \frac{RW_{alt,k}}{(1+i)^k} \right) - RW_{alt,0}}_{\text{Beitrag der Weiternutzung der alten Anlage}} + \underbrace{\frac{KW_{neu}}{(1+i)^k}}_{\text{Beitrag der neuen Anlage ab Jahr k}} $$
*(Für $S_0$ (sofortiger Ersatz): $KW_{S0} = RW_{alt,0} + KW_{neu}$)*

**Tabellarische Darstellung der Strategie-Zahlungsströme (wie in deiner Dozenten-Lösung zu ÜA19 für einen festen Planungshorizont $T_{plan}$ und $AN_{neu}$):**

| Strategie ($S_k$)      | Zahlung t=0                  | Zahlung t=1                                       | ... | Zahlung t=k                                       | Zahlung t=k+1 | ... | Zahlung t=$T_{plan}$ | $KW_{Sk}$ bei i |
| :--------------------- | :--------------------------- | :------------------------------------------------ | :-- | :------------------------------------------------ | :------------ | :-- | :------------------- | :-------------- |
| **$S_0$ (Ersatz t=0)** | $+RW_{alt,0}$                | $AN_{neu}$                                        | ... | $AN_{neu}$ (falls k=$T_{plan}$)                     | $AN_{neu}$    | ... | $AN_{neu}$           | **Berechnen**   |
| **$S_1$ (Ersatz t=1)** | $-RW_{alt,0}$                | $CF_{alt,1} + RW_{alt,1}$                         | ... | $AN_{neu}$ (falls k+1=$T_{plan}$)                   | $AN_{neu}$    | ... | $AN_{neu}$           | **Berechnen**   |
| ...                    | ...                          | ...                                               | ... | ...                                               | ...           | ... | ...                  | ...             |
| **$S_{Tplan}$ (Nie Ersatz im Plan.Hor.)** | $-RW_{alt,0}$ | $CF_{alt,1}$                                      | ... | $CF_{alt,Tplan} + RW_{alt,Tplan}$                 | -             |     | -                    | **Berechnen**   |

---

**3. Optimales Investitionsprogramm (Dean-Modell bei Kapitalrationierung)**

*Entscheidungskriterium: Realisiere Projekte, deren **IRR > Kosten der Finanzierung** sind, bis das Budget erschöpft ist oder keine profitablen Projekte mehr verfügbar sind.*

**3.1. Vorgehen (Tabellarisch):**
1.  **Projekte:** Nach fallendem IRR ordnen.
    | Projekt | $I_0$ | IRR (%) |
    | :------ | :---- | :------ |
    | A       | ...   | ...     |
    | B       | ...   | ...     |
2.  **Finanzierungsquellen:** Nach steigenden Kosten (Zinssatz $i_{FK}$) ordnen.
    | Quelle | Volumen | Kosten (%) |
    | :----- | :------ | :--------- |
    | EK     | ...     | $i_{EK}$ (Opp.K.) |
    | FK1    | ...     | $i_{FK1}$  |
3.  **Matching:** Projekte mit günstigsten Finanzierungsquellen finanzieren, solange IRR > Finanzierungskosten.
    *   *Beispielhafte Entscheidungstabelle (wie Folie 80):*
        | Finanzierungs-mittel | Max. Betrag | Sollzins | Investitions-vorhaben | Kapital-einsatz | Interne Verzinsung | Optimales Budget (Projekt, Betrag) |
        | :------------------- | :---------- | :------- | :-------------------- | :-------------- | :----------------- | :--------------------------------- |
        | Quelle 1             | ...         | ...      | Projekt X             | ...             | ...                | Projekt X, ...                     |
        | ...                  | ...         | ...      | Projekt Y (ggf. teilw.)| ...             | ...                | Projekt Y (teilw.), ...            |

---

**4. (Einfacher) Finanzplan**

*Zweck: Systematische Erfassung aller Zahlungsströme zur Ermittlung einer Zielgröße (z.B. Endwert).*

**4.1. Grundstruktur/Wichtige Zeilen (Schema):**

| Position                 | Ende Jahr 0 | Ende Jahr 1    | Ende Jahr 2    | ... | Ende Jahr n             |
| :----------------------- | :---------- | :------------- | :------------- | :-- | :---------------------- |
| CF Investitionsobjekt    | -$I_0$      | $CF_1$         | $CF_2$         | ... | $CF_n + RW_n$           |
| +/- EK-Einlage/Entnahme  | +EK         | (ggf.Entnahme) | (ggf.Entnahme) | ... | (ggf.End-EK)            |
| +/- FK-Aufnahme/Tilgung  | +FK         | (Tilgung)      | (Tilgung)      | ... | -(Rest-FK + Tilgung)    |
| - FK-Zinsen              |             | -$Z_1$         | -$Z_2$         | ... | -$Z_n$                  |
| **Saldo vor Disposition**| **$S_0$**   | **$S_1$**      | **$S_2$**      | ... | **$S_n$**               |
| +/- Finanzanlage/Kredit  | -$S_0$ (wenn $S_0$>0 anlegen) | -$S_1$ (wenn $S_1$>0 anlegen) | ... | ... | +Endwert Finanzanlagen  |
| **Saldo nach Disposition**| **0**       | **0**          | **0**          | ... | **Endwert des Projekts**|
*(Hinweis: Bei Anlage von $S_t$ fließen $S_t \times (1+i_H)^{n-t}$ am Ende der Periode n wieder zu).*
