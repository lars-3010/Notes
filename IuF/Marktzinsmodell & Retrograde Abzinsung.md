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

*   **Grundidee Marktzinsmodell (Folie 89):**
    *   **Abkehr vom einheitlichen Kalkulationszins:** Stattdessen Verwendung *aktueller, laufzeitabhängiger Marktzinssätze* (Zinsstrukturkurve).
    *   **Realistischere Bewertung:** Spiegelt die tatsächlichen Finanzierungs- und Anlagekonditionen am Markt besser wider.
    *   **Konsequente Einzelbewertung:** Investitionen werden isoliert betrachtet.

*   **Retrograde Abzinsung (Folie 91-92):**
    *   **Notwendigkeit:** Bei laufzeitabhängigen Zinsen kann man nicht einfach jeden Cashflow mit *seinem* laufzeitbezogenen Spot-Zins auf t=0 abzinsen. Man muss "rückwärts" durch die Zeit gehen.
    *   **Prinzip:**
        1.  Die letzte Zahlung (CFn) wird mit dem 1-Jahres-Zinssatz, der für die Periode von n-1 bis n gilt, auf den Zeitpunkt n-1 abgezinst.
        2.  Dieser Barwert wird zum CF(n-1) addiert.
        3.  Diese Summe wird mit dem 1-Jahres-Zinssatz, der für die Periode von n-2 bis n-1 gilt, auf den Zeitpunkt n-2 abgezinst.
        4.  Usw., bis man bei t=0 ankommt. Der dort verbleibende Wert ist der Kapitalwert unter Marktzinsmodell-Annahmen.
    *   **Deine Folien 92-94 zeigen die tabellarische Umsetzung:** Die "Eliminierung" der letzten Zahlung durch Aufnahme eines fiktiven Kredits, dessen Barwert und Zinskosten in die vorherigen Perioden eingearbeitet werden, ist die praktische Umsetzung dieses Prinzips.
    *   **Für die Klausur (Hinweis verstehen):** Verstehe, *warum* man retrograd vorgeht (wegen der unterschiedlichen Zinsen für unterschiedliche Restlaufzeiten) und das *Grundprinzip* des schrittweisen Abzinst und Addierens. Die Detailrechnung der Zinskosten in den Bearbeitungszeilen ist komplex; das Ergebnis in der ersten Spalte (Kapitalwert) ist das Ziel.
