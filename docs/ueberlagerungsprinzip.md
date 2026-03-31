# Das Überlagerungsprinzip (Superpositionsprinzip)

Das Überlagerungsprinzip (auch Superpositionsprinzip oder Überlagerungssatz von Helmholtz) ist ein grundlegendes Verfahren zur Analyse linearer elektrischer Netzwerke mit mehreren Quellen.

---

## 1. Grundprinzip

### 1.1 Definition

In einem **linearen elektrischen Netzwerk** mit mehreren unabhängigen Quellen ist die Wirkung einer einzelnen Quelle gleich der Summe der Wirkungen aller einzelnen Quellen, wenn diese nacheinander allein wirken.

**Mathematisch:**
I_ges = I_1 + I_2 + I_3 + ...
U_ges = U_1 + U_2 + U_3 + ...

### 1.2 Gültigkeitsbedingungen

Das Überlagerungsprinzip gilt nur für **lineare** Netzwerke, das heißt:

- Alle Bauelemente müssen **ohmsche Widerstände** sein (R = konstant)
- Keine nichtlinearen Elemente wie Dioden, Transistoren im Arbeitsbereich
- Die Netzwerkgleichungen müssen linear sein

### 1.3 Vorteile des Verfahrens

- Vereinfacht die Berechnung komplexer Schaltungen
- Jede Quelle wird einzeln analysiert
- Ergebnisse werden am Ende addiert
- Besonders nützlich bei Schaltungen mit vielen Quellen

---

## 2. Anwendung des Überlagerungsprinzips

### 2.1 Schritt-für-Schritt-Vorgehen

1. **Alle Quellen bis auf eine entfernen:**
   - Spannungsquellen: Kurzschließen (U = 0)
   - Stromquellen: Öffnen (I = 0)

2. **Teillösung berechnen:**
   - Berechne alle gesuchten Ströme/Spannungen mit nur einer Quelle

3. **Wiederholen für jede Quelle:**
   - Für jede Quelle die Schritte 1-2 wiederholen

4. **Ergebnisse überlagern:**
   - Alle Teillösungen algebraisch addieren
   - Vorzeichen beachten!

### 2.2 Beispiel: Schaltung mit zwei Spannungsquellen

**Gegeben:**
- U1 = 10 V, U2 = 5 V
- R1 = 2 Ohm, R2 = 3 Ohm, R3 = 5 Ohm

**Gesucht:** Strom I3 durch R3

**Schritt 1:** Nur U1 wirkt (U2 kurzgeschlossen)

R_ersatz = R2 || R3 = (3 x 5)/(3 + 5) = 1,875 Ohm
R_ges = R1 + R_ersatz = 2 + 1,875 = 3,875 Ohm
I_ges = U1 / R_ges = 10 V / 3,875 Ohm = 2,58 A

Mit Stromteilerregel:
I3' = I_ges x (R2 / (R2 + R3)) = 2,58 x (3/8) = 0,97 A

**Schritt 2:** Nur U2 wirkt (U1 kurzgeschlossen)

R_ersatz = R1 || R3 = (2 x 5)/(2 + 5) = 1,43 Ohm
R_ges = R2 + R_ersatz = 3 + 1,43 = 4,43 Ohm
I_ges = U2 / R_ges = 5 V / 4,43 Ohm = 1,13 A

I3'' = I_ges x (R1 / (R1 + R3)) = 1,13 x (2/7) = 0,32 A

**Schritt 3:** Überlagerung

I3 = I3' - I3'' = 0,97 A - 0,32 A = 0,65 A
(Das Minus, weil U2 entgegengesetzt wirkt)

---

## 3. Überlagerungsprinzip mit Stromquellen

### 3.1 Vorgehensweise

Bei Stromquellen:
- **Stromquelle entfernen:** Unterbrechen (kein Strompfad)
- **Spannungsquelle entfernen:** Kurzschließen

### 3.2 Beispiel: Gemischte Quellen

**Gegeben:**
- U = 12 V
- I = 2 A
- R1 = 4 Ohm, R2 = 6 Ohm, R3 = 3 Ohm

**Gesucht:** Spannung U3 über R3

**Schritt 1:** Nur U wirkt (I-Quelle unterbrochen)

R_ges = R1 + R2 + R3 = 4 + 6 + 3 = 13 Ohm
I = U / R_ges = 12/13 = 0,92 A
U3' = I x R3 = 0,92 x 3 = 2,77 V

**Schritt 2:** Nur I wirkt (U-Quelle kurzgeschlossen)

Parallelschaltung von R1 mit R2+R3:
R_ges = R1 x (R2 + R3) / (R1 + R2 + R3) = 4 x 9/13 = 2,77 Ohm

I teilt sich im Verhältnis der Leitwerte:
U3'' = I x (R1 x (R2 + R3) / (R1 + R2 + R3))
U3'' = 2 x 2,77 = 5,54 V

**Schritt 3:** Überlagerung

U3 = U3' + U3'' = 2,77 V + 5,54 V = 8,31 V

---

## 4. Leistung und Überlagerungsprinzip

### 4.1 Wichtiger Hinweis

**Achtung:** Das Überlagerungsprinzip gilt NICHT für die Leistung!

P ist ungleich P_1 + P_2

Die Leistung muss aus dem Gesamtstrom bzw. der Gesamtspannung berechnet werden:

P_ges = I_ges^2 x R = U_ges^2 / R

### 4.2 Warum nicht für Leistung?

Die Leistung ist eine **quadratische** Funktion des Stroms:

P = I^2 x R

(I_1 + I_2)^2 = I_1^2 + I_2^2 + 2 x I_1 x I_2 ist ungleich I_1^2 + I_2^2

Der Mischterm 2 x I_1 x I_2 darf nicht vernachlässigt werden.

---

## 5. Vergleich mit anderen Methoden

| Methode | Vorteile | Nachteile | Anwendungsfall |
|---------|---------|-----------|----------------|
| **Überlagerung** | Einfach bei vielen Quellen | Zeitaufwändig bei vielen Quellen | Netzwerke mit 2-3 Quellen |
| **Knotenpotential** | Systematisch, gut für Computer | Gleichungssystem nötig | Viele Knoten, wenige Maschen |
| **Maschenstrom** | Systematisch | Gleichungssystem nötig | Viele Maschen, wenige Knoten |
| **Thevenin/Norton** | Vereinfacht Teilschaltungen | Zusätzlicher Aufwand | Lastabhängige Analysen |

---

## 6. Anwendungen in der biomedizinischen Technik

### 6.1 EKG-Messung

Bei der EKG-Ableitung überlagern sich die elektrischen Signale verschiedener Herzabschnitte:

- P-Welle: Vorhofdepolarisation
- QRS-Komplex: Kamm depolarisation
- T-Welle: Kammer repolarisation

### 6.2 Brückenschaltungen mit Kompensation

In Messbrücken kann das Überlagerungsprinzip zur Kompensation von Nullabgleich verwendet werden.

### 6.3 Verstärkerschaltungen

Bei Operationsverstärkern in linearen Schaltungen überlagern sich Eingangssignale und Offset-Spannungen.

---

## 7. Zusammenfassung

- Das Überlagerungsprinzip gilt nur für **lineare** Netzwerke
- Jede Quelle wird **einzeln** analysiert
- Ergebnisse werden **algebraisch addiert**
- Spannungsquellen werden **kurzgeschlossen**
- Stromquellen werden **unterbrochen**
- **NICHT** für Leistungsberechnung anwendbar
