# Formaler Lösungsweg

In komplexen Stromnetzwerken reicht das reine Anwenden von Serien- und Parallelschaltung nicht aus. Stattdessen kommt ein systematischer, **formaler Lösungsweg** zum Einsatz – etwa durch das Aufstellen und Lösen eines **Gleichungssystems** auf Basis von Kirchhoff-Regeln.

---

## 1. Ziel des Verfahrens

- **Systematische Berechnung** aller Ströme und Spannungen
- **Unabhängig von Anordnung** oder Komplexität der Schaltung
- Vorbereitung für automatisierte Simulationen und numerische Lösungsverfahren

---

## 2. Vorgehensweise

1. Zählpfeile für Ströme und Spannungen festlegen
2. Benennung aller Zweigströme und -spannungen
3. Aufstellen von:
   - **Knotengleichungen (KCL)**: \( k - 1 \) Stück
   - **Maschengleichungen (KVL)**: \( z - k + 1 \) Stück
   - **Ohmsche Gesetze**: für jeden Zweig
4. Zusammenführen in ein Gleichungssystem
5. Lösung über Einsetzungsverfahren, Gleichungsmatrix oder Software

---

## 3. Anzahl der Gleichungen

| Bezeichnung              | Formel                                 |
|--------------------------|-----------------------------------------|
| Anzahl Unbekannter       | \( 2z \) (je Strom und Spannung pro Zweig) |
| Knotengleichungen        | \( k - 1 \)                            |
| Maschengleichungen       | \( z - k + 1 \)                        |
| Ohmsche Gleichungen      | \( z \)                                |
| Gesamtanzahl Gleichungen | \( (k-1) + (z-k+1) + z = 2z \)         |

➡️ Es gibt **genauso viele Gleichungen wie Unbekannte** – das Gleichungssystem ist lösbar.

---

## 4. Beispielstruktur

Gegeben:
- 3 Zweige: \( I_1, I_2, I_3 \)
- 2 Knoten
- 2 Maschen

**Gleichungssystem:**
1. \( -I_1 + I_2 + I_3 = 0 \) (Knotenregel)
2. \( U_1 - U_2 = 0 \) (Maschenregel)
3. \( U_2 - U_3 = 0 \)
4. \( U_1 = R_1 \cdot I_1 \)
5. \( U_2 = R_2 \cdot I_2 \)
6. \( U_3 = R_3 \cdot I_3 \)

---

## 5. Darstellung als Matrix

Das Gleichungssystem kann in **Matrixform** überführt werden:

\[
A \cdot \vec{x} = \vec{b}
\]

Beispielhafte Struktur:
- \( \vec{x} = [U_1, U_2, U_3, I_1, I_2, I_3]^T \)
- \( A \): Koeffizientenmatrix
- \( b \): Ergebnisspalte (z. B. \( [0, 0, 0, U_q, 0, 0]^T \))

➡️ Die Lösung erfolgt rechnerisch oder mit Tools wie Python, Matlab, Octave.

---

## 6. Werkzeuge zur Lösung

- Manuell (Gleichungssystem von Hand lösen)
- CAS-Rechner (TI-Nspire, ClassPad)
- Tabellenkalkulation (Excel, LibreOffice Calc)
- MATLAB, Octave
- Python (z. B. mit `numpy.linalg.solve`)
- LTspice (grafisch + rechnerisch)

---

## 7. Weiterführende Links

- [Kirchhoff-Regeln – vertiefend (Wikipedia)](https://de.wikipedia.org/wiki/Kirchhoffsches_Gesetz)
- [Gleichungssysteme lösen – YouTube (Mathe by Daniel Jung)](https://www.youtube.com/watch?v=8G3PjRUsXCM)
- [Python NumPy `linalg.solve`](https://numpy.org/doc/stable/reference/generated/numpy.linalg.solve.html)