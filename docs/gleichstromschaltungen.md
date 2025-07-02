# Gleichstromschaltungen

In diesem Kapitel lernst du, wie man komplexere Gleichstromschaltungen analysiert, indem man sie in **Zweige**, **Knoten** und **Maschen** unterteilt. Du erfährst, wie man mithilfe von Spannungsteiler-, Stromteiler- und Kirchhoff-Gesetzen Ströme und Spannungen berechnet.

---

## 1. Grundbegriffe

### Zweig
- Ein durchgehender Leitungsabschnitt ohne Abzweigung.
- Alle Bauteile im Zweig sind **in Serie** geschaltet.
- Es fließt **derselbe Strom** durch alle Bauteile.

### Knoten
- Verbindungsstelle von mindestens **drei Zweigen**.
- Die **Summe der zufließenden und abfließenden Ströme ist null**.

  $$ \sum I = 0 $$

### Masche
- Geschlossener Stromkreisweg in einer Schaltung.
- Die **Summe der Spannungen** in einer Masche ist null.

  $$ \sum U = 0 $$

---

## 2. Beispielschaltung

Eine Beispielschaltung besteht aus:
- einer idealen Spannungsquelle \( U_q \)
- sechs Widerständen \( R_1 \) bis \( R_6 \)

Diese lassen sich in drei Zweige aufteilen:
- Zweig 1: \( R_1 \), \( R_5 \)
- Zweig 2: \( R_3 \)
- Zweig 3: \( R_2 \), \( R_4 \), \( R_6 \)

---

## 3. Spannungsteiler

Spannung wird auf zwei in Serie geschaltete Widerstände aufgeteilt:

$$ U_1 = U_{ges} \cdot \frac{R_1}{R_1 + R_2} $$

$$ U_2 = U_{ges} \cdot \frac{R_2}{R_1 + R_2} $$

➡️ Anwendung: z. B. zur Einstellung von Bezugsspannungen

---

## 4. Stromteiler

Ein Gesamtstrom wird auf parallele Widerstände aufgeteilt:

$$ I_1 = I_{ges} \cdot \frac{R_2}{R_1 + R_2} $$

$$ I_2 = I_{ges} \cdot \frac{R_1}{R_1 + R_2} $$

➡️ Anwendung: z. B. zur Signalaufteilung oder Lastverteilung

---

## 5. Kirchhoffsche Gesetze

### Knotenregel (KCL)

Die Summe aller Ströme an einem Knoten ist null:

$$ \sum I = 0 $$

### Maschenregel (KVL)

Die Summe aller Spannungen in einer geschlossenen Masche ist null:

$$ \sum U = 0 $$

Diese Regeln gelten unabhängig vom Zählpfeilsystem – wichtig ist die **Vorzeichengenauigkeit**!

---

## 6. Beispiel: Teilspannung berechnen


![Reihenschaltung](images/gleichstrom-serienschaltung.png){: .small-img }

Gesucht: Spannung an \( R_4 \)

1. Rechne \( R_2 + R_4 + R_6 \) als Serienschaltung zusammen
2. Diese Gruppe ist parallel zu \( R_3 \)
3. Verwende Spannungsteiler, um \( U_4 \) zu berechnen:

$$ U_4 = U_q \cdot \frac{R_4}{R_2 + R_4 + R_6} $$

---

## 7. Beispiel: Teilstrom berechnen

Gesucht: Strom durch den Zweig \( R_2 + R_4 + R_6 \)

1. Berechne Gesamtwiderstand \( R_{ges} \)
2. Bestimme Gesamtstrom \( I_q = \frac{U_q}{R_{ges}} \)
3. Verwende Stromteiler:

$$ I_{Zweig} = I_q \cdot \frac{R_3}{R_3 + (R_2 + R_4 + R_6)} $$

---

## 8. Weiterführende Links

- [Kirchhoffsche Regeln – Wikipedia](https://de.wikipedia.org/wiki/Kirchhoffsches_Gesetz)
- [Maschenregel und Knotenregel erklärt – YouTube (simpleclub)](https://www.youtube.com/watch?v=Z7JvYv7SsmU)
- [LTspice (kostenloses Simulationsprogramm für Stromkreise)](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html)