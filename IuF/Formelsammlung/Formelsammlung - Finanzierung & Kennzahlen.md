---
tags:
  - 🌱
"up::":
  - "[[../../../../Projects/Courses/_Investition und Finanzierung|_Investition und Finanzierung]]"
  - "[[Formelsammlung - Optimierungsansätze & Sonderfälle]]"
similar:
leads to:
contradicts:
extends:
implements:
reviewed:
sources:
---
**1. Grundlagen Finanzierung (A-Priorität für Verständnis, keine tiefen Rechenaufgaben erwartet)**

*   **1.1. Investition vs. Finanzierung (Folie 112 - A)**
    *   **Investition:** Mittelverwendung (Geldkapital -> Realkapital). Ziel: Ertrag/Nutzen.
    *   **Finanzierung:** Mittelherkunft (Kapitalbeschaffung). Ziel: Zahlungsfähigkeit, Investitionen ermöglichen.
    *   *Wichtig: Sind zwei Seiten einer Medaille.*
*   **1.2. Innen- vs. Außenfinanzierung (Folie 114 - A)**
    *   **Innenfinanzierung:** Kapital aus dem Unternehmen selbst.
        *   **Selbstfinanzierung:** Aus einbehaltenen Gewinnen. (A)
        *   **Finanzierung aus Abschreibungsgegenwerten:** "Verdiente" Abschreibungen. (A - Basis für Lohmann-Ruchti)
        *   *Finanzierung aus Rückstellungsgegenwerten (B-Priorität, Folie 118):* Mittel aus Rückstellungen.
    *   **Außenfinanzierung:** Kapital von außen.
        *   **Beteiligungsfinanzierung (Eigenfinanzierung):** Einlagen/Aktien. (A)
        *   **Kreditfinanzierung (Fremdfinanzierung):** Kredite/Anleihen. (A)
*   **1.3. Cash-Flow-Finanzierung (Folie 118 - A)**
    *   **Konzept:** Finanzierung aus dem internen Zahlungsmittelüberschuss. Umfasst im Wesentlichen die Finanzierung aus Gewinnen und Abschreibungen.

**2. Lohmann-Ruchti-Effekt (A-Priorität für Rechenanwendung und Verständnis)**

*   **2.1. Kurze Erklärung (Folie 120, 124 - A):** Kapazitätserweiterung durch kontinuierliche Reinvestition der durch Abschreibungen freigesetzten liquiden Mittel in *zusätzliche* (gleichartige) Anlagen, bevor die alten ersetzt werden müssen.
*   **2.2. Wichtige Spalten der LR-Tabelle (für Rechenaufgaben):**
    *   Jahr
    *   Anzahl Fertigungsanlagen (Anfangsbestand + Zugänge - Abgänge)
    *   Investiertes Kapital (Anzahl Anlagen * AW pro Anlage)
    *   Abschreibung (Gesamtabschreibung aller Anlagen im Park)
    *   Reinvestition (Wie viele *neue* Anlagen können aus `Abschreibung + Abschreibungsrest Vorjahr` gekauft werden? Ergebnis *Anzahl neuer Anlagen* x AW pro Anlage)
    *   Abschreibungsrest (Liquide Mittel aus Abschreibungen, die nicht sofort reinvestiert werden konnten = `Abschreibung + Abschreibungsrest Vorjahr - Reinvestition`)
    *   Zugänge an Anlagen (Anzahl neuer Anlagen aus Reinvestition)
    *   Abgänge an Anlagen (Anzahl Anlagen, die das Ende ihrer ND erreichen)
    *   Anlagen Saldo (Veränderung der Anzahl der Anlagen = Zugänge - Abgänge)
    *   *Voraussetzungen (Folie 120):* verdiente Abschreibungen, sofortige Reinvestition, konstante Preise, gleiche ND & Produktivität.
    *   *Effekte (Folie 120):* Kapitalfreisetzungseffekt, Kapazitätserweiterungseffekt.

**3. Wichtige Finanzkennzahlen (A-Priorität für Berechnung und Interpretation)**

*   **3.1. ROI-System (DuPont) (Folie 129 - A, Folie 28-30 - C für Basis)**
    *   **ROI-Formel:** $ROI = \frac{\text{Gewinn (vor FK-Zinsen)}}{\text{Durchschn. Gesamtkapital}} \times 100\%$
    *   **Zerlegung:** $ROI = \underbrace{\left(\frac{\text{Gewinn}}{\text{Umsatz}}\right)}_{\text{Umsatzrentabilität (UR)}} \times \underbrace{\left(\frac{\text{Umsatz}}{\text{Durchschn. Gesamtkapital}}\right)}_{\text{Kapitalumschlag (KU)}}$
    *   *Anwendung: Analyse der Rentabilitätstreiber.*
*   **3.2. Liquiditätsgrade (Folie 137 - A für Anwendung, B für tiefere Interpretation)**
    *   **Liquidität 1. Grades (Barliquidität):**
        $ L1 = \frac{\text{Flüssige Mittel}}{\text{Kurzfristige Verbindlichkeiten}} \times 100\% $
        *(Sollte kurzfristige Zahlungsverpflichtungen zumindest teilweise decken können).*
    *   **Liquidität 2. Grades (Einzugsliquidität / Quick Ratio):**
        $ L2 = \frac{\text{Flüssige Mittel + Kurzfristige Forderungen}}{\text{Kurzfristige Verbindlichkeiten}} \times 100\% $
        *(Sollte ca. 100% betragen, um fristgerechte Zahlung ohne Verkauf von Vorräten zu gewährleisten).*
    *   **Liquidität 3. Grades (Umsatzliquidität / Current Ratio):**
        $ L3 = \frac{\text{Gesamtes Umlaufvermögen}}{\text{Kurzfristige Verbindlichkeiten}} \times 100\% $
        *(Sollte deutlich über 100% liegen, da auch langsam drehende Vorräte enthalten sind).*

**4. Unternehmensbewertung (Grundlagen – WACC konzeptionell, Folie 146, 148 - B)**

*   **4.1. WACC-Formel (Folie 146 - B für Verständnis der Formel, Anwendung wie Folie 148/149 ist A/B):**
    $$ WACC = \frac{EK_M}{GK_M} \cdot k_{EK} + \frac{FK_M}{GK_M} \cdot k_{FK} \cdot (1-s) $$
    *Wobei $EK_M, FK_M, GK_M$ = Marktwerte; $k_{EK}, k_{FK}$ = Kosten für EK/FK; $s$ = Steuersatz.*
    *Verständnis: WACC als gewichteter Durchschnittskostensatz für Kapital, der als Diskontsatz für (freie) Cashflows bei der Unternehmens- oder Projektbewertung dienen kann (wenn Risiko ähnlich).*
*   **4.2. Schema zur Berechnung freier Zahlungsüberschüsse und Abzinsung mit WACC (ähnlich Folie 148/149 - A/B):**
    *   EBIT
    *   - Steuern auf EBIT (fiktiv, als ob rein EK-finanziert)
    *   = NOPAT (Net Operating Profit After Tax)
    *   + Abschreibungen
    *   - Investitionen ins Anlagevermögen
    *   +/- Veränderung Working Capital
    *   = Free Cash Flow (FCF)
    *   Diese FCFs werden dann mit dem WACC aufsummiert zum Unternehmenswert.
    *   *Für Klausur: Eher Anwendung des gegebenen WACC auf gegebene Cashflows, weniger die Herleitung des FCF im Detail, es sei denn, es ist eine klare Rechenaufgabe dazu da.*

---

**TEIL 5: KONZEPTIONELLES VERSTÄNDNIS (Klausurrelevanter Fokus A & B)**

**1. Marktzinsmodell & Retrograde Abzinsung (Folie 89 - B, 91-94 - A für "Hinweis verstehen")**
*   **Warum?** Berücksichtigung laufzeitabhängiger Marktzinssätze statt eines einheitlichen Kalkulationszinses -> realistischer.
*   **Prinzip der retrograden Abzinsung:** "Rückwärts" durch die Zeit abzinsen, weil der Zinssatz für eine Periode von der dann geltenden (Rest-)Laufzeit abhängt. (Tabellarische Methode wie auf Folie 92/93 als "Hinweis verstehen", d.h. die Logik der Verrechnung, nicht jede Zinsdetailrechnung).

**2. Sensitivitätsanalyse (Folie 111 - A für "Idee verstehen")**
*   **Was?** Untersuchung, wie stark sich das Ergebnis einer Investitionsrechnung (z.B. KW) ändert, wenn *einzelne* Input-Größen (Preis, Menge, Kosten etc.) variiert werden.
*   **Warum?** Identifikation kritischer Faktoren, Risikoabschätzung.
