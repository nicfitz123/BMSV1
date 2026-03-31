# Elektrische Messverfahren

Die elektrische Messtechnik umfasst die Bestimmung von Strom, Spannung, Widerstand und Leistung. Diese Grundmessungen sind die Basis für alle elektronischen und biomedizinischen Messungen.

---

## 1. Messung der elektrischen Spannung

### 1.1 Prinzip der Spannungsmessung

Die Spannung wird immer **parallel** zum Messobjekt angeschlossen. Ein idealer Spannungsmesser hat einen **unendlich hohen Eingangswiderstand**, sodass er den Messkreis nicht beeinflusst.

R → ∞ (Eingangswiderstand gegen unendlich)

### 1.2 Messgeräte

**Digitalmultimeter (DMM):**
- Hohe Eingangsimpedanz (R_in > 1 MΩ)
- Anzeige als Zahlenwert
- Typischer Fehler: ±(0,1% + 1 Digit)

**Oszilloskop:**
- Darstellung des zeitlichen Verlaufs
- Gleich- und Wechselspannung
- Hochohmiger Tastkopf (R_in = 1 MΩ)

### 1.3 Spannungsmessung mit dem Oszilloskop

U_eff = U_SS / (2 × √2)

Dabei ist U_SS die Spitze-zu-Spitze-Spannung.

### 1.4 Messfehler bei der Spannungsmessung

**Belastungsfehler:** Wenn der Eingangswiderstand des Messgeräts zu niedrig ist, wird die Schaltung belastet.

U_mess = U_orig × (R_in / (R_in + R_innen))

**Lösung:** Spannungsmesser mit hoher Eingangsimpedanz verwenden.

---

## 2. Messung des elektrischen Stroms

### 2.1 Prinzip der Strommessung

Der Strom wird immer **in Reihe** (seriell) in den Messkreis eingefügt. Ein idealer Strommesser hat den **Widerstand Null**.

R → 0

### 2.2 Messgeräte

**Analoges Zeigerinstrument:**
- Drehspulmesswerk
- Empfindlichkeit in Ω/V angegeben

**Digitalmultimeter:**
- Direkte Anzeige in A, mA, µA
- Interner Shunt-Widerstand

**Stromzange (Clamp-Meter):**
- Berührungslose Strommessung
- Nutzt magnetische Wirkung des Stroms

### 2.3 Messbereichserweiterung

Mit einem **Shunt-Widerstand** kann der Messbereich erweitert werden:

I_ges = I_mess + I_Shunt

R_Shunt = U_mess / I_Shunt

---

## 3. Messung des elektrischen Widerstands

### 3.1 Methoden der Widerstandsmessung

**a) Ohmsches Gesetz:**
R = U / I

**b) Spezifische Messverfahren:**

| Methode | Prinzip | Anwendungsbereich |
|---------|---------|-------------------|
| Spannungsmethode | R = U/I | Mittlere Widerstände |
| Wheatstone-Brücke | Abgleichmethode | Präzise Messung |
| Digitalmultimeter | Eingebauter Konstantstrom | Universell |
| Vierleitermessung | Eliminierung der Zuleitungswiderstände | Sehr kleine Widerstände |

### 3.2 Wheatstone-Brücke

Die Wheatstone-Brücke ist eine Präzisionsmessmethode:

R1/R2 = R3/R4 → R_x = R_N × (R2/R1)

**Abgleich:** Widerstand R4 wird so eingestellt, dass die Brückenspannung U_B = 0 wird.

### 3.3 Vierleitermessung (Kelvin-Methode)

Bei sehr kleinen Widerständen (< 1 Ω) müssen die Zuleitungswiderstände eliminiert werden:

- **Stromkreise:** Zuführung des Messstroms über separate Leitungen
- **Messkreise:** Spannungsabfall wird direkt am Widerstand abgegriffen

R_mess = U_mess / I_mess

---

## 4. Messung der elektrischen Leistung

### 4.1 Grundgleichungen

**Gleichstromleistung:**
P = U × I = I² × R = U² / R

**Einheiten:**
- 1 W = 1 V × 1 A
- 1 kW = 1000 W
- 1 MW = 10^6 W

### 4.2 Leistungsmessung mit Wattmeter

Ein Wattmeter misst gleichzeitig Strom und Spannung:

P = U_eff × I_eff × cos(φ)

Dabei ist φ der Phasenwinkel zwischen Strom und Spannung.

### 4.3 Leistungsmessung mit DMM

**Methode 1:** Separates Messen von U und I
P = U × I

**Methode 2:** Strom und Spannung gleichzeitig messen

### 4.4 Leistung bei Wechselstrom

**Wirkleistung:** P = U_eff × I_eff × cos(φ)

**Blindleistung:** Q = U_eff × I_eff × sin(φ)

**Scheinleistung:** S = U_eff × I_eff

---

## 5. Messfehler und Unsicherheiten

### 5.1 Systematische Fehler

- **Gerätefehler:** Kalibrierungsabweichungen
- **Belastungsfehler:** Einfluss des Messgeräts auf die Schaltung
- **Temperaturfehler:** Temperatureinfluss auf Bauteile

### 5.2 Zufällige Fehler

- Rauschen
- Kontaktwiderstände
- Umgebungseinflüsse

### 5.3 Fehlerrechnung

**Absolute Unsicherheit:**
ΔR = ± (ΔR/R × 100% + Digit)

**Relative Unsicherheit:**
ΔR / R

**Beispiel:** DMM zeigt R = 1000 Ω mit Fehler ±(0,5% + 2 Digits) und Auflösung 0,1 Ω:
ΔR = ±(0,5% × 1000 Ω + 2 × 0,1 Ω) = ±(5 Ω + 0,2 Ω) = ± 5,2 Ω

---

## 6. Praktische Hinweise für die Messtechnik

### 6.1 Messbereichswahl

- Immer mit dem **größten Messbereich** beginnen
- Dann auf den kleinsten Bereich schalten, der noch einen guten Zeigerausschlag/Displaywert liefert
- Bei DMM: Messbereich nie überschreiten (Bereichsautomatik bevorzugen)

### 6.2 Innenwiderstand beachten

| Messgerät | Typischer Innenwiderstand |
|-----------|--------------------------|
| Analoges Voltmeter | 20 kΩ/V |
| Digitalmultimeter | > 1 MΩ |
| Oszilloskop | 1 MΩ |
| Strommessung DMM | Shunt: mΩ bis Ω |

### 6.3 Sicherheitshinweise

- Messgeräte auf den richtigen Messbereich einstellen
- Bei hohen Spannungen spezielle Hochspannungstastköpfe verwenden
- NIEMALS den Strommessbereich eines DMM als Spannungsmessbereich verwenden
