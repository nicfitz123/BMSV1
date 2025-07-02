# Biosignale

Biosignale sind physikalische oder chemische Veränderungen im menschlichen Körper, die als Grundlage für Diagnostik, Therapieüberwachung oder Forschung dienen. Sie lassen sich in verschiedene Arten und Kategorien einteilen – je nach Trägermedium und Signalcharakteristik.

---

## 1. Was ist ein Signal?

Ein **Signal** ist eine Darstellung von Information über eine physikalische Größe. Die Information ist dabei in bestimmten **Signalparametern** kodiert – typischerweise abhängig von der Zeit (zeitabhängige Funktion).

Beispiele:
- Spannung über die Zeit (z. B. EKG)
- Temperaturverlauf
- Frequenz eines Tones

Weiterführend: [Wikipedia: Signal (Technik)](https://de.wikipedia.org/wiki/Signal_(Technik))

---

## 2. Was sind Biosignale?

**Biosignale** sind Signale, die vom menschlichen (oder tierischen) Körper erzeugt werden. Sie resultieren aus physiologischen Prozessen und können verschiedene physikalische oder chemische Formen annehmen.

### Typische Trägermedien:

- **Elektrisch** – z. B. Gehirnaktivität (EEG), Herzaktivität (EKG)
- **Mechanisch** – z. B. Druck im Gefäßsystem, Bewegungen
- **Akustisch** – z. B. Herztöne, Atemgeräusche
- **Thermisch** – z. B. Körpertemperatur
- **Chemisch** – z. B. pH-Wert des Blutes
- **Olfaktorisch** – z. B. Körpergeruch (selten genutzt, aber medizinisch relevant)

---

## 3. Elektrische Biosignale

Elektrische Biosignale sind in der Medizintechnik am weitesten verbreitet. Sie entstehen durch **ionischen Stromfluss** in Nervenzellen oder Muskeln.

### Beispiele:

| Biosignal | Beschreibung | Anwendung |
|-----------|--------------|-----------|
| **EKG** (Elektrokardiogramm) | misst Herzaktivität | Kardiologie |
| **EEG** (Elektroenzephalogramm) | misst Gehirnströme | Neurologie, Schlafmedizin |
| **EMG** (Elektromyogramm) | misst Muskelaktivität | Neurologie, Reha |
| **EOG** (Elektrookulogramm) | misst Augenbewegungen | Augenheilkunde, HCI |

Diese Signale sind oft im Bereich von **µV bis mV**.

Weiterführend:
- [Wikipedia: Elektrokardiogramm (EKG)](https://de.wikipedia.org/wiki/Elektrokardiogramm)
- [Wikipedia: Elektroenzephalografie (EEG)](https://de.wikipedia.org/wiki/Elektroenzephalografie)

---

## 4. Mechanische und andere Biosignale

Mechanische Signale resultieren aus Kräften, Bewegungen und Drücken im Körper. Typische Anwendungen:

- **Blutdruck**: gemessen mit Manschette oder invasiv
- **Kieferbewegung**: z. B. beim Kauen
- **Pulswelle**: Ausbreitungsgeschwindigkeit des Blutdrucks

### Weitere Kategorien:

- **Akustisch**: z. B. Stethoskop zur Auskultation
- **Thermisch**: Infrarot-Thermografie, Hauttemperatur
- **Chemisch**: Sensoren für pH, Sauerstoffsättigung, Glukose (z. B. CGM bei Diabetes)
- **Olfaktorisch**: selten instrumentell erfasst, aber biologisch bedeutsam

---

## 5. Messkette bei Biosignalen

Der Weg vom biologischen Ursprungssignal bis zur digitalen Auswertung:

1. **Biosignal** (z. B. Spannung, Druck)
2. **Sensor** (z. B. Elektroden, Dehnungsmessstreifen)
3. **Messwandler** (z. B. Brückenschaltung, elektromechanisch)
4. **Verstärker** (z. B. Instrumentenverstärker mit hoher Gleichtaktunterdrückung)
5. **Analog-Digital-Wandler (ADC)** – z. B. im Mikrocontroller
6. **Digitale Signalverarbeitung** (Filter, Mittelwert, Fourier)
7. **Anzeige / Speicherung**

Mehr dazu: [Signalverarbeitung medizinischer Daten (TU Darmstadt)](https://www.bmt.tu-darmstadt.de/)

---

## 6. Herausforderungen bei der Messung

- **Störungen & Rauschen**: Netzbrummen, EMV-Einflüsse, Bewegungsartefakte
- **Signalstärke**: oft sehr schwach (µV), daher hohe Verstärkung nötig
- **Kontaktprobleme**: z. B. Elektrodenqualität
- **Interpretation**: Variabilität zwischen Personen

Typische Gegenmaßnahmen:
- Differenzielle Messung
- Abschirmung
- Filterung (Tiefpass, Hochpass, Notch)

---

## 7. Warum Biosignalverarbeitung?

- **Diagnosehilfe**: Krankheiten frühzeitig erkennen
- **Therapieüberwachung**: z. B. bei Herzschrittmachern
- **Assistive Systeme**: z. B. Brain-Computer-Interfaces
- **Forschung**: z. B. emotionale Zustände aus EEG ableiten