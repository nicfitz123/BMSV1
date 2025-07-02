# Elektrische Größen

Dieses Kapitel vermittelt die Grundlagen elektrischer Größen, wie sie in der Elektronik und speziell in der Biosignalverarbeitung auftreten. Es werden Strom, Spannung, Leistung, Energie und Widerstand behandelt – sowohl physikalisch als auch rechnerisch.

---

## 1. Elektrizität und Ladung

- Elektrizität beruht auf der Bewegung von **elektrischen Ladungsträgern** (Elektronen, Ionen).
- Es gibt **positive** und **negative** Ladungen.
- Gleichnamige Ladungen stoßen sich ab, ungleichnamige ziehen sich an.
- Ladungsträger bewegen sich in einem **elektrischen Feld**.
- Jede Materie enthält Ladungsträger – meist Elektronen oder Ionen.

---

## 2. Leiterklassen

| Klasse             | Beschreibung |
|--------------------|--------------|
| **Leiter 1. Klasse** | Metalle mit frei beweglichen Elektronen („Elektronengas“) |
| **Leiter 2. Klasse** | Elektrolyte mit beweglichen Ionen (z. B. in biologischen Flüssigkeiten) |

➡️ In der Biomedizin sind oft Leiter 2. Klasse relevant (z. B. Gewebe, Blut).

---

## 3. Elektrischer Strom (I)

- **Definition**: Bewegung von elektrischen Ladungsträgern
- Einheit: **Ampere [A]**
- Formel:  
  $$ I = \frac{Q}{t} $$
  wobei:
  - *I* = Strom
  - *Q* = transportierte Ladung [C]
  - *t* = Zeit [s]

- Bei Gleichstrom ist die **Driftgeschwindigkeit** der Elektronen sehr klein (~0.1 mm/s), dennoch wird Information praktisch mit Lichtgeschwindigkeit übertragen.

---

## 4. Elektrische Spannung (U)

- **Definition**: Potenzialdifferenz zwischen zwei Punkten
- Einheit: **Volt [V]**
- Spannung ist die **Ursache** für das Fließen von Strom.
- Formel:  
  $$ U = W / Q $$
  wobei:
  - *W* = Energie [J]
  - *Q* = Ladung [C]

➡️ Spannungsquellen (z. B. Batterien, Biozellen) liefern diese Potenzialdifferenz.

---

## 5. Elektrische Energie (E)

- **Definition**: Fähigkeit, elektrische Arbeit zu verrichten
- Einheit: **Joule [J] = Wattsekunde [Ws]**
- In biologischen Systemen ist oft die chemisch gespeicherte Energie entscheidend (z. B. ATP in Zellen).

Formel:
$$ E = P \cdot t $$

---

## 6. Elektrische Leistung (P)

- **Definition**: Umgesetzte Energie pro Zeit
- Einheit: **Watt [W]**
- Formel:
  $$ P = U \cdot I $$

  Auch:
  $$ P = I^2 \cdot R \,\text{ oder }\, P = \frac{U^2}{R} $$

➡️ Leistungsgrößen sind wichtig zur Bewertung von Verlusten, Wärmeentwicklung und Energieverbrauch.

---

## 7. Elektrischer Widerstand (R)

- **Definition**: Maß für den Widerstand gegen den Stromfluss
- Einheit: **Ohm [Ω]**
- Formel (Ohmsches Gesetz):  
  $$ R = \frac{U}{I} $$

- Widerstand ist **materialabhängig** und **temperaturabhängig**.

Beispielhafte Werte:
- Hautwiderstand: mehrere kΩ (je nach Feuchtigkeit)
- Leiterbahnen: mΩ
- Isolatoren: GΩ

---

## 8. Übersicht: Formelzeichen und Einheiten

| Größe        | Formelzeichen | Einheit     |
|--------------|----------------|-------------|
| Spannung     | U              | Volt (V)    |
| Strom        | I              | Ampere (A)  |
| Widerstand   | R              | Ohm (Ω)     |
| Energie      | E              | Joule (J)   |
| Leistung     | P              | Watt (W)    |

---

## 9. Grundgleichungen

- Ohmsches Gesetz:  
  $$ U = R \cdot I $$
  $$ I = \frac{U}{R} $$
  $$ R = \frac{U}{I} $$

- Leistung:
  $$ P = U \cdot I = I^2 \cdot R = \frac{U^2}{R} $$

- Energie:
  $$ E = P \cdot t $$

---

## Weiterführende Links

- [Ohmsches Gesetz – Wikipedia](https://de.wikipedia.org/wiki/Ohmsches_Gesetz)
- [Elektrische Leistung – Simpleclub Video (YouTube)](https://www.youtube.com/watch?v=gMgCQJeLTvk)
- [Leiter und Isolatoren – Erklärung](https://de.wikipedia.org/wiki/Leiter_(Physik))