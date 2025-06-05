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
[[]]#### **1.1. Abzinsung (Diskontierung)**

*   **Ziel:** Den heutigen Wert (Barwert) einer zukünftigen Zahlung ermitteln.
*   **Name:** Abzinsungsfaktor (AFt) / Diskontierungsfaktor
*   **Formel (für eine Zahlung in t Perioden):**
    $$ AF_t = \frac{1}{(1+i)^t} = (1+i)^{-t} $$
    *Wobei:*
    *   `i` = Kalkulationszinssatz pro Periode (als Dezimalzahl)
    *   `t` = Anzahl der Perioden in der Zukunft
*   **Kurzerklärung:** Multiplikator, um den Wert einer zukünftigen Zahlung auf den heutigen Zeitpunkt "herunterzurechnen".

*   **Name:** Barwert (BW) / Present Value (PV)
*   **Formel (einer einzelnen zukünftigen Zahlung CFt):**
    $$ BW_t = CF_t \times AF_t = CF_t \times (1+i)^{-t} = \frac{CF_t}{(1+i)^t} $$
    *Wobei:*
    *   `CFt` = Cashflow (Zahlung) am Ende der Periode t
*   **Kurzerklärung:** Der Wert, den eine in der Zukunft liegende Zahlung heute besitzt, wenn man mit dem Kalkulationszinssatz `i` rechnet.

#### **1.2. Aufzinsung (seltener direkt für Klausurrechnung benötigt, aber wichtig für das Verständnis des Zinseszinseffekts und für Endwertberechnungen bei Finanzplänen)**

*   **Ziel:** Den zukünftigen Wert einer heutigen Zahlung ermitteln.
*   **Name:** Aufzinsungsfaktor (ZFt) / Endwertfaktor
*   **Formel (für eine Zahlung heute auf t Perioden in der Zukunft):**
    $$ ZF_t = (1+i)^t $$
*   **Name:** Endwert (EW) / Future Value (FV)
*   **Formel (einer einzelnen heutigen Zahlung CF₀):**
    $$ EW_t = CF_0 \times ZF_t = CF_0 \times (1+i)^t $$
*   **Kurzerklärung:** Der Wert, den eine heutige Zahlung in `t` Perioden unter Berücksichtigung von Zins und Zinseszins haben wird.

**Wichtiger Hinweis zu den Tabellen (z.B. aus der Klausur):**
In Klausuren werden oft Tabellen mit Abzinsungsfaktoren (Diskontierungsfaktoren) für verschiedene Zinssätze und Laufzeiten bereitgestellt. Du musst diese Faktoren dann nur noch korrekt ablesen und anwenden.