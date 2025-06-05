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
**Ziel (allgemein):** Ermittlung eines Wertes für ein gesamtes Unternehmen oder für Eigenkapitalanteile.
**Fokus laut deiner Priorisierung:** Hier geht es NICHT um die detaillierte Durchführung einer Unternehmensbewertung, sondern um das **Verständnis der WACC-Formel als Diskontierungszinssatz** und die Grundidee, wie Unternehmenswerte aus zukünftigen Cashflows abgeleitet werden könnten. Deine Folie 148 zeigt ein *Rechenbeispiel zur Anwendung des WACC auf Cashflows*, was ein Hinweis auf diesen Anwendungsfokus ist.

*   **Weighted Average Cost of Capital (WACC):**
    *   **Name:** WACC / Gewichtete durchschnittliche Kapitalkosten
    *   **Formel (Folie 146):**
        $$ WACC = \frac{EK_M}{GK_M} \cdot k_{EK} + \frac{FK_M}{GK_M} \cdot k_{FK} \cdot (1-s) $$
        *Wobei:*
        *   $EK_M, FK_M, GK_M$: Marktwerte von Eigen-, Fremd- und Gesamtkapital.
        *   $k_{EK}$: Eigenkapitalkostensatz (Renditeforderung der EK-Geber, oft über CAPM bestimmt).
        *   $k_{FK}$: Fremdkapitalkostensatz (Zinssatz für Fremdkapital).
        *   $s$: Ertragssteuersatz des Unternehmens (wegen steuerlicher Abzugsfähigkeit der FK-Zinsen – "Tax Shield").
    *   **Kurzerklärung:** Der WACC stellt die durchschnittlichen Kapitalkosten eines Unternehmens dar, gewichtet nach dem Anteil von Eigen- und Fremdkapital an der Gesamtfinanzierung. Er wird oft als Diskontierungszinssatz für die Bewertung von Projekten oder ganzen Unternehmen verwendet, die eine ähnliche Risikostruktur wie das Gesamtunternehmen aufweisen.

*   **Unternehmenswert-Grundidee (Discounted Cash Flow - DCF-Ansatz mit WACC):**
    *   Der Wert eines Unternehmens (oder Projekts) ergibt sich aus dem Barwert seiner zukünftig erwarteten freien Cashflows (FCF), abgezinst mit dem WACC.
    *   **Formel (Grundprinzip, siehe Folie 146 unten):**
        $$ UW_0 = \sum_{t=1}^{T} \frac{E(FCF_t)}{(1+WACC)^t} + \frac{\text{Terminal Value}_T}{(1+WACC)^T} $$
        *Wobei E(FCFt) der erwartete Free Cash Flow in Periode t ist und der Terminal Value den Wert aller Cashflows nach der Detailplanungsperiode T darstellt.*
    *   **Dein Beispiel auf Folie 148/149:** Zeigt die Berechnung von "Freien Zahlungsüberschüssen" (ähnlich FCF) und deren Abzinsung mit einem gegebenen WACC, um einen Unternehmenswert zu ermitteln. Das *Schema der Cashflow-Ermittlung* und die *Anwendung des WACC zur Abzinsung* sind hier das Wichtige.

**Für die Klausur (Fokus):**
*   Die **WACC-Formel verstehen** und die Komponenten benennen können.
*   Das **Prinzip verstehen**, dass der WACC als gewichteter Kapitalkostensatz dient und zur Abzinsung von Cashflows bei der Unternehmens-/Projektbewertung verwendet werden kann.
*   Ein **einfaches Schema zur Ermittlung freier Cashflows und deren Abzinsung mit WACC** (wie Folie 148/149) nachvollziehen und anwenden können, wenn die Werte gegeben sind.
*   (CAPM auf Folie 147 ist eher Hintergrundwissen zur Bestimmung von $k_{EK}$, nicht unbedingt für eine direkte Rechenaufgabe).
*   Andere Bewertungsverfahren (Ertragswert, Mischverfahren auf Folie 140, 144, 143) sind laut deiner C-Priorisierung eher konzeptionell, falls überhaupt.
