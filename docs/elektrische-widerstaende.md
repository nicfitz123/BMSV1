# Elektrische Widerstände

Der elektrische Widerstand beschreibt, wie stark der Fluss von elektrischem Strom durch ein Material behindert wird. Dieses Kapitel behandelt Grundlagen, Formeln und Temperaturabhängigkeit sowie praktische Anwendungen wie NTC- und PTC-Widerstände.

---

## 1. Definition

- Der **elektrische Widerstand** (R) ist das Verhältnis zwischen Spannung und Strom.
- Formel nach dem Ohmschen Gesetz:

  $$ R = \frac{U}{I} $$

- Einheit: **Ohm (Ω)**

Ein hoher Widerstand bedeutet, dass bei gegebener Spannung nur ein kleiner Strom fließt.

---

## 2. Widerstand eines Leiters

Der Widerstand eines Drahts oder Leiters hängt von seinen physikalischen Eigenschaften ab:

$$ R = \rho \cdot \frac{l}{A} $$

| Symbol | Bedeutung                  |
|--------|----------------------------|
| \( R \)    | elektrischer Widerstand       |
| \( \rho \) | spezifischer Widerstand (Materialkonstante) |
| \( l \)    | Länge des Leiters            |
| \( A \)    | Querschnittsfläche des Leiters |

Beispielwerte:
- Kupfer: \( \rho \approx 0{,}0178 \ \Omega \cdot mm^2/m \)
- Aluminium: \( \rho \approx 0{,}028 \ \Omega \cdot mm^2/m \)

---

## 3. Temperaturabhängigkeit

Metalle und Halbleiter verhalten sich unterschiedlich bei Temperaturänderungen.

### Lineare Abhängigkeit (Metalle)

$$ R = R_{20} \cdot (1 + \alpha \cdot \Delta T) $$

| Symbol     | Bedeutung                            |
|------------|----------------------------------------|
| \( R_{20} \)  | Widerstand bei 20 °C                  |
| \( \alpha \) | Temperaturkoeffizient (1/K)         |
| \( \Delta T \) | Temperaturänderung in Grad Celsius |

Typische \( \alpha \)-Werte:
- Kupfer: 0.00393 1/K
- Wolfram: 0.0046 1/K

---

## 4. NTC und PTC

### PTC – Kaltleiter
- **Positive Temperature Coefficient**
- \( \alpha > 0 \)
- Widerstand **steigt** mit Temperatur
- Typisch bei Metallen

### NTC – Heißleiter
- **Negative Temperature Coefficient**
- \( \alpha < 0 \)
- Widerstand **sinkt** mit Temperatur
- Typisch bei Halbleitern (z. B. Thermistoren)

Nichtlineare Formel für NTC:
$$ R = R_{20} \cdot e^{B\left(\frac{1}{T} - \frac{1}{T_0}\right)} $$

mit:
- \( T_0 = 293{,}15 \ K \) (20 °C)
- \( B \): Materialkonstante

---

## 5. Anwendungen

- **PTC**: Sicherungen, Temperaturschutz
- **NTC**: Temperaturmessung, Einschaltstrombegrenzung
- **Heizdrähte**: Widerstandsheizung (abhängig von Material und Länge)
- **Biologische Sensorik**: Thermistoren in medizinischer Messtechnik

---

## 6. Zusammenfassung

| Typ        | Verhalten bei Temperatur | Anwendung                   |
|------------|---------------------------|------------------------------|
| PTC        | Widerstand steigt         | Temperatursicherung, Sensorik |
| NTC        | Widerstand sinkt          | Temperaturmessung, Regelung  |

---

## Weiterführende Links

- [Wikipedia: Elektrischer Widerstand](https://de.wikipedia.org/wiki/Elektrischer_Widerstand)
- [Thermistor – NTC/PTC Grundlagen (YouTube)](https://www.youtube.com/watch?v=kMY5nYEC0FY)
- [NTC/PTC im Alltag – Conrad](https://www.conrad.de/de/ratgeber/elektronik/ntc-ptc.html)