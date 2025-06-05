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
(Folie 54!!)

**Das Kernproblem:** Bei der Auswahl zwischen mehreren, sich gegenseitig ausschließenden Investitionsprojekten können KW-Methode und IRR-Methode zu unterschiedlichen Rangfolgen und somit zu unterschiedlichen optimalen Entscheidungen führen.

**Ursache: Unterschiedliche Wiederanlageprämissen**

*   **Kapitalwertmethode (KW):** Unterstellt implizit, dass alle während der Projektlaufzeit anfallenden Rückflüsse zum **Kalkulationszinssatz (i)** wiederangelegt werden können.
    *   *Argument dafür:* Der Kalkulationszinssatz repräsentiert oft die Opportunitätskosten des Kapitals oder die durchschnittliche Rendite alternativer Anlagen am Markt. Diese Prämisse wird häufig als realistischer angesehen.
*   **Interner Zinsfuß Methode (IRR):** Unterstellt implizit, dass alle während der Projektlaufzeit anfallenden Rückflüsse zum **projektindividuellen Internen Zinsfuß (IRR)** wiederangelegt werden können.
    *   *Problem damit:* Wenn ein Projekt einen sehr hohen IRR hat (z.B. 50%), ist es oft unrealistisch anzunehmen, dass die daraus generierten Rückflüsse wieder zu 50% angelegt werden können. Meist ist die Wiederanlagemöglichkeit eher beim Marktzins (Kalkulationszinssatz i) zu finden.

**Wann tritt der Konflikt typischerweise auf?**

*   Bei Projekten mit stark unterschiedlichen **Höhen der Anschaffungsauszahlung**.
*   Bei Projekten mit stark unterschiedlichen **zeitlichen Strukturen der Rückflüsse** (z.B. ein Projekt mit hohen frühen Rückflüssen, ein anderes mit hohen späten Rückflüssen).
*   Bei Projekten mit stark unterschiedlichen **Nutzungsdauern** (obwohl hier die Annuitätenmethode oft besser zum Vergleich geeignet ist).

**Entscheidungsempfehlung bei Konflikt:**

*   **Generell wird der Kapitalwertmethode der Vorzug gegeben**, da ihre Wiederanlageprämisse (Anlage zum Kalkulationszinssatz i) als marktkonformer und realistischer gilt. Der Kapitalwert misst direkt den Vermögenszuwachs in Euro zum Entscheidungszeitpunkt.
*   **Der IRR kann irreführend sein**, insbesondere bei der Auswahl zwischen Projekten, da er eine relative Rendite darstellt und nichts über den absoluten Vermögenszuwachs aussagt. Ein kleines Projekt mit hohem IRR kann weniger zum Gesamtvermögen beitragen als ein großes Projekt mit einem etwas niedrigeren, aber immer noch guten IRR.

**Lösungsansatz zur Analyse des Konflikts (Verständnis, nicht unbedingt tiefe Rechnung in Klausur, außer es wird explizit verlangt und geübt):**

*   **Analyse der Differenzinvestition:**
    1.  Bilde die Zahlungsreihe der Differenzinvestition zwischen den beiden Projekten (Zahlungsreihe Projekt A minus Zahlungsreihe Projekt B).
    2.  Berechne den IRR dieser Differenzinvestition (IRRDiff).
    3.  Vergleiche IRRDiff mit dem Kalkulationszinssatz (i):
        *   Wenn **IRRDiff > i**: Die "Mehrinvestition" (die das eine Projekt gegenüber dem anderen darstellt) ist vorteilhaft. Dies stützt die Entscheidung der Kapitalwertmethode (das Projekt mit dem höheren KW ist tatsächlich besser, weil die zusätzliche Investition sich über i hinaus lohnt).
        *   Wenn **IRRDiff < i**: Die "Mehrinvestition" ist nicht vorteilhaft. Auch dies hilft, die KW-Entscheidung zu verstehen.

**Kritischer Zinssatz (Schnittpunkt der Kapitalwertprofile):**
Es gibt einen bestimmten Zinssatz (den "kritischen Zinssatz" oder "Fisher's Intersection"), bei dem die Kapitalwerte beider Projekte gleich sind.
*   Liegt der Kalkulationszinssatz (i) **unterhalb** dieses kritischen Zinssatzes, kann die Rangfolge nach IRR und KW unterschiedlich sein.
*   Liegt der Kalkulationszinssatz (i) **oberhalb** dieses kritischen Zinssatzes, führen KW und IRR oft zur gleichen Rangfolge.
    (Die grafische Darstellung auf Folie 53 illustriert dies).

**Für die Klausur (Fokus):**
*   **Kenne die Wiederanlageprämissen beider Methoden!**
*   **Wisse, dass der KW-Methode bei widersprüchlichen Ergebnissen meist der Vorzug gegeben wird und warum (realistischere Wiederanlageprämisse).**
*   Verstehe die Ursachen, warum es zu Konflikten kommen kann (unterschiedliche Kapitaleinsätze, Zahlungsstromprofile).
*   Die Berechnung der Differenzinvestition ist eher ein fortgeschrittenes Konzept; das grundlegende Verständnis des Problems und der Lösungsempfehlung ist wichtiger.

# Zusatz
---
**Kern des Konflikts:** Unterschiedliche Wiederanlageprämissen.

- KW: Wiederanlage zum Kalkulationszinssatz i.
    
- IRR: Wiederanlage zum projekteigenen IRR.
    

**Beispielhafte Zahlungsreihen, die zu einem Konflikt führen könnten:**

**Projekt A (Hohe frühe Rückflüsse):**  
I₀ = -1000  
CF₁ = 700  
CF₂ = 300  
CF₃ = 300

**Projekt B (Hohe späte Rückflüsse, evtl. höherer Kapitaleinsatz):**  
I₀ = -1200  
CF₁ = 200  
CF₂ = 400  
CF₃ = 1000

Bei einem bestimmten Kalkulationszinssatz i (z.B. 5%) könnte Projekt A einen höheren KW haben.  
Projekt A könnte aber auch einen höheren IRR haben als Projekt B.  
Bei einem anderen Kalkulationszinssatz i (z.B. 15%) könnte sich die Rangfolge nach KW ändern, während die Rangfolge nach IRR gleich bleibt.

**Analyse der Differenzinvestition (Konzept für Verständnis):**  
Man bildet die Zahlungsreihe (A-B) oder (B-A) und berechnet deren IRR (IRRDiff).

Zahlungsreihe (A-B):  
I₀(A-B) = -1000 - (-1200) = +200 (Projekt B ist initial "teurer")  
CF₁(A-B) = 700 - 200 = +500  
CF₂(A-B) = 300 - 400 = -100  
CF₃(A-B) = 300 - 1000 = -700

(Achtung: Die Interpretation der Differenzinvestition kann komplex sein, je nachdem, welches Projekt die höhere Anfangsauszahlung hat. Für die Klausur ist das Verständnis wichtig, dass die KW-Methode meist bevorzugt wird).

**Entscheidung:** (Wie oben genannt)  
Im Konfliktfall wird meist der **Kapitalwertmethode der Vorzug** gegeben, da ihre Wiederanlageprämisse als realistischer gilt.

**Grafische Darstellung (siehe Folie 53 der Präsentation):**  
Die Kapitalwertprofile zweier Projekte (KW in Abhängigkeit vom Zinssatz i) können sich schneiden. Der Schnittpunkt ist der "kritische Zinssatz" (Fisher's Intersection).

- Links vom Schnittpunkt: Ein Projekt hat den höheren KW.
    
- Rechts vom Schnittpunkt: Das andere Projekt kann den höheren KW haben.
    
- Die Rangfolge nach IRR bleibt davon unberührt (es sei denn, es gibt multiple IRRs, was aber meist nicht Klausurfokus ist).
    

**Für die Klausur ist entscheidend:**

- Die **Wiederanlageprämissen** nennen und erklären können.
    
- Begründen können, warum dem **KW meist der Vorzug** gegeben wird.
    
- Erkennen, dass unterschiedliche Zahlungsstromprofile oder Kapitaleinsätze zu Konflikten führen können.