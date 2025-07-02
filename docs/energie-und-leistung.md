# Energie und Leistung

In elektrischen Schaltungen spielt der Energieverbrauch und die abgegebene Leistung eine zentrale Rolle – nicht nur für die Dimensionierung von Bauteilen, sondern auch im Hinblick auf Effizienz, Wärmeentwicklung und Sicherheit.

---

## 1. Elektrische Leistung (P)

- Definition: **Energieumsatz pro Zeit**
- Einheit: **Watt (W)**
- Formeln:

  $$ P = U \cdot I $$
  $$ P = I^2 \cdot R $$
  $$ P = \frac{U^2}{R} $$

Diese Formeln sind für Gleichstrom gültig.

### Beispiel:

Ein Widerstand von \( R = 100 \ \Omega \) wird mit \( U = 10 \ V \) betrieben:

$$ P = \frac{U^2}{R} = \frac{100}{100} = 1 \ W $$

➡️ Es wird 1 Watt in Wärme umgewandelt.

---

## 2. Elektrische Energie (E)

- Definition: **Arbeit**, die durch elektrischen Strom verrichtet wird
- Einheit: **Joule (J)** oder **Wattsekunde (Ws)**

Formel:

$$ E = P \cdot t $$

Dabei ist:
- \( P \): elektrische Leistung in Watt
- \( t \): Zeit in Sekunden

---

## 3. Energieeinheiten im Alltag

| Einheit         | Umrechnung                         | Anwendung                    |
|------------------|-------------------------------------|-------------------------------|
| 1 Joule (J)       | 1 Watt × 1 Sekunde                  | physikalische Grundgröße     |
| 1 kWh             | 1000 W × 3600 s = 3.6 Mio J         | Stromrechnung, Haushalt      |
| 1 cal             | 4.1868 J                            | Lebensmittel (veraltet)      |

➡️ Auf Stromrechnungen wird die **Kilowattstunde (kWh)** verwendet.

---

## 4. Zusammenhang aller Größen

Diagrammartige Zusammenfassung:

```
   U
   |        P = U * I
   ↓
   I → R = U / I → P = I² * R
   ↓
   P → E = P * t
```

➡️ Mit zwei bekannten Werten kannst du alle anderen berechnen!

---

## 5. Bedeutung in der Praxis

- **Leistung**:
  - Dimensionierung von Bauteilen (z. B. Widerstände mit 0.25 W, 0.5 W)
  - Wärmeentwicklung berücksichtigen!
- **Energie**:
  - Akkukapazität (z. B. in mAh → rechnerisch in Wh)
  - Stromverbrauch von Geräten einschätzen

---

## 6. Beispiel: Stromverbrauch

Ein medizinisches Gerät verbraucht **2 W** und läuft täglich **3 Stunden**.

Berechnung der Energie:

$$ E = P \cdot t = 2 \cdot (3 \cdot 3600) = 21.600 \ J = 6 \ Wh $$

---

## 7. Weiterführende Links

- [Elektrische Energie – Wikipedia](https://de.wikipedia.org/wiki/Elektrische_Energie)
- [Leistung und Energie – YouTube (simpleclub)](https://www.youtube.com/watch?v=xCkN4ts5J3U)
- [Umrechnung J → kWh, Wh, cal](https://www.umrechnung.org/energie/joule-kilowattstunde-umrechnen.htm)