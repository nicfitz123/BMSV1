# Gleichstromwiderstandsnetze

Gleichstromwiderstandsnetze bestehen aus mehreren Widerständen, die in einem Stromkreis miteinander verbunden sind. Sie lassen sich analysieren, indem man sie in Serien- und Parallelschaltungen auflöst und mit dem Ohmschen Gesetz berechnet.

---

## 1. Grundlagen und Ziele

- Analyse von Netzwerken mit mehreren Widerständen
- Ziel: Berechnung von Gesamtwiderständen, Teilströmen und Teilspannungen
- Methoden:
  - Ohmsches Gesetz
  - Serien- und Parallelschaltung
  - Ersatzwiderstände bilden

---

## 2. Vorsilben für Zehnerpotenzen

| Zahl           | Potenz   | Vorsilbe |
|----------------|----------|----------|
| 1 000 000 000  | 10⁹      | Giga (G) |
| 1 000 000      | 10⁶      | Mega (M) |
| 1 000          | 10³      | Kilo (k) |
| 0.001          | 10⁻³     | Milli (m) |
| 0.000001       | 10⁻⁶     | Mikro (µ) |
| 0.000000001    | 10⁻⁹     | Nano (n) |

➡️ Diese Vorsilben werden oft bei Widerstandswerten (z. B. kΩ, MΩ) verwendet.

---

## 3. Serienschaltung

- Der Strom ist in allen Bauteilen gleich.
- Spannungen addieren sich:

  $$ R_{ges} = R_1 + R_2 + ... + R_n $$

**Beispiel:**
Zwei Widerstände in Serie:

```text
[ R1 ] — [ R2 ]
```

Wenn \( R_1 = 100 \ \Omega \), \( R_2 = 200 \ \Omega \), dann:

\( R_{ges} = 300 \ \Omega \)

---

## 4. Parallelschaltung

- Die Spannung ist in allen Zweigen gleich.
- Ströme teilen sich auf.
- Kehrwertregel:

  $$ \frac{1}{R_{ges}} = \frac{1}{R_1} + \frac{1}{R_2} + ... + \frac{1}{R_n} $$

Für zwei Widerstände:

  $$ R_{ges} = \frac{R_1 \cdot R_2}{R_1 + R_2} $$

**Beispiel:**
\( R_1 = 100 \ \Omega \), \( R_2 = 200 \ \Omega \):

\( R_{ges} = 66{,}7 \ \Omega \)

---

## 5. Gemischte Schaltung

- Kombination aus Serien- und Parallelschaltung
- Vorgehen:
  1. Parallele Widerstände zu Ersatzwiderständen zusammenfassen
  2. Serienwiderstände addieren
  3. Schrittweise reduzieren

➡️ Schrittweise Vereinfachung bis zum Gesamtwiderstand

---

## 6. Spannungsteiler

Teilt eine Spannung auf zwei in Serie geschaltete Widerstände auf.

Formeln:
- Gesamtspannung: \( U = U_1 + U_2 \)
- Teilschritte:

  $$ U_1 = U \cdot \frac{R_1}{R_1 + R_2} $$
  $$ U_2 = U \cdot \frac{R_2}{R_1 + R_2} $$

Anwendung: Spannungsanpassung, Sensorbeschaltung

---

## 7. Stromteiler

Teilt einen Strom auf zwei parallele Widerstände auf.

Formeln:

  $$ I_1 = I_{ges} \cdot \frac{R_2}{R_1 + R_2} $$
  $$ I_2 = I_{ges} \cdot \frac{R_1}{R_1 + R_2} $$

➡️ Der kleinere Widerstand erhält den größeren Stromanteil.

---

## 8. Zählpfeile und Systeme

- **Spannungszählpfeile**: zeigen vom Plus zum Minus
- **Stromzählpfeile**: zeigen in angenommene Stromrichtung
- **Erzeugerzählpfeilsystem (EZS)**: U und I zeigen entgegengesetzt
- **Verbraucherzählpfeilsystem (VZS)**: U und I zeigen in dieselbe Richtung

Negatives Ergebnis bei Berechnung → Pfeilrichtung falsch angenommen

---

## 9. Schaltungssymbole

| Symbol      | Bedeutung              |
|-------------|------------------------|
| [ ⎍ ]       | Spannungsquelle (ideal) |
| [ → ]       | Stromquelle (ideal)     |
| [ —[R]— ]   | Widerstand              |
| [ —[R(T)]— ]| temperaturabhängiger Widerstand (NTC/PTC) |

---

## 10. Weiterführende Links

- [Widerstandsnetzwerke – Wikipedia](https://de.wikipedia.org/wiki/Widerstandsnetzwerk)
- [Reihenschaltung und Parallelschaltung – Simpleclub (YouTube)](https://www.youtube.com/watch?v=BFX1FzEp1xI)
- [Spannungsteiler interaktiv simulieren – Falstad](https://www.falstad.com/circuit/)