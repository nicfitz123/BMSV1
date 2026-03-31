# Sensoren in der Biomedizinischen Technik

Sensoren sind Wandler, die physikalische, chemische oder biologische Größen in elektrische Signale umwandeln. In der biomedizinischen Technik werden sie zur Erfassung von Biosignalen und Umgebungsparametern eingesetzt.

---

## 1. Mechanische Sensoren

Mechanische Sensoren wandeln mechanische Größen wie Kraft, Druck, Dehnung oder Beschleunigung in elektrische Signale um.

### 1.1 Dehnungsmessstreifen (DMS)

**Funktionsprinzip:** Ein DMS besteht aus einem dünnen Leiter (typischerweise Konstantan), der auf ein Trägermaterial aufgebracht ist. Bei Dehnung ändert sich der elektrische Widerstand proportional zur Dehnung.

 \frac{\Delta R}{R} = k \cdot \frac{\Delta l}{l} 

Dabei ist $ der **k-Faktor** (typisch:  \approx 2$ für Metall-DMS).

**Anwendung in der Medizintechnik:**
- Blutdruckmessung (DMS in Dehnungsmessstreifen-Sensoren)
- Kraftmessung in Orthesen und Prothesen
- Atemfrequenzmessung (Dehnungssensoren im Gurt)

### 1.2 Drucksensoren

**Piezoelektrische Sensoren:**
- Erzeugen eine elektrische Ladung bei mechanischer Belastung
- Geeignet für dynamische Druckänderungen
- Anwendung: Herz-Kreislauf-Monitoring, Ultraschall

**Kapazitive Drucksensoren:**
- Ändern ihre Kapazität bei Druckänderung
- Hohe Empfindlichkeit
- Anwendung: intrakranielle Druckmessung

### 1.3 Beschleunigungssensoren

**Piezo-resistive Beschleunigungssensoren:**
- Nutzen die Widerstandsänderung von Halbleitermaterialien
- Anwendung: Vibrationsanalyse, Bewegungserkennung

**Kapazitive MEMS-Beschleunigungssensoren:**
- Micromechanische Systeme
- Anwendung: Schrittzähler, Sturzerkennung in Wearables

---

## 2. Widerstandssensoren

Widerstandssensoren nutzen die Abhängigkeit des elektrischen Widerstands von einer Messgröße.

### 2.1 Dehnungsmessstreifen (Widerstandsprinzip)

Siehe Abschnitt 1.1 - DMS sind klassische Widerstandssensoren.

### 2.2 Thermistoren (NTC/PTC)

**NTC-Widerstand (Negative Temperature Coefficient):**
 R_T = R_0 \cdot e^{\beta \left( \frac{1}{T} - \frac{1}{T_0} \right)} 

- Widerstand nimmt mit steigender Temperatur ab
- Anwendung: Temperaturmessung in medizinischen Geräten

**PTC-Widerstand (Positive Temperature Coefficient):**
- Widerstand nimmt mit steigender Temperatur zu
- Anwendung: Überlastschutz, Temperaturalarm

### 2.3 Fotowiderstand (LDR)

- Widerstand sinkt bei Belichtung
- Anwendung: Optische Sensoren, Pulsoximetrie

### 2.4 Potentiometer

- Lineare oder rotatorische Widerstandsänderung
- Anwendung: Positionsmessung, Winkelsensoren

---

## 3. Thermosensoren

Thermosensoren erfassen Temperaturänderungen und wandeln sie in elektrische Signale um.

### 3.1 Thermoelemente

**Funktionsprinzip:** Zwei unterschiedliche Metalle erzeugen bei Temperaturdifferenz eine elektrische Spannung (Seebeck-Effekt).

 U = S_{AB} \cdot \Delta T 

Dabei ist {AB}$ der Seebeck-Koeffizient des Thermoelementpaares.

**Typen und Anwendungen:**

| Typ | Temperaturbereich | Anwendung |
|-----|------------------|-----------|
| Typ K | -200°C bis +1350°C | Industrielle Anwendungen |
| Typ T | -250°C bis +350°C | Medizintechnik, Kühlschränke |
| Typ E | -40°C bis +900°C | Hochpräzise Messungen |

### 3.2 Widerstandsthermometer (RTD)

**Funktionsprinzip:** Nutzen den positiven Temperaturkoeffizienten von Platin.

 R_T = R_0 \cdot (1 + \alpha \cdot \Delta T) 

- Hohe Genauigkeit und Langzeitstabilität
- Pt100-Sensor:  = 100\,\Omega$ bei ^\circ
- $\alpha \approx 0.00385\,\text{K}^{-1}$ für Pt

**Anwendung:**
- Präzise Körpertemperaturmessung
- Inkubatoren und Wärmetherapie
- Laborgeräte

### 3.3 Infrarot-Thermometer

**Funktionsprinzip:** Messen die Infrarotstrahlung, die von der Oberfläche abgestrahlt wird.

 P = \varepsilon \cdot \sigma \cdot A \cdot T^4 

- Nicht-kontakt Messung
- Anwendung: Ohr-/Stirnthermometer, industrielle Temperaturkontrolle

### 3.4 Halbleiter-Temperatursensoren

- Integrierte Schaltungen mit linearer Kennlinie
- Ausgangsspannung proportional zur Temperatur
- Anwendung: Mikrocontroller-Systeme, Patientenüberwachung

---

## 4. Sensorauswahl für biomedizinische Anwendungen

### Kriterien:

1. **Genauigkeit:** Je nach Anwendung sind unterschiedliche Genauigkeiten erforderlich
2. **Ansprechzeit:** Schnelle Änderungen erfordern Sensoren mit kurzer Ansprechzeit
3. **Linearität:** Wünschenswert für einfache Kalibrierung
4. **Stabilität:** Langzeitstabilität für kontinuierliche Überwachung
5. **Biokompatibilität:** Für implantierbare Sensoren essentiell

### Vergleichstabelle:

| Sensortyp | Messgröße | Empfindlichkeit | Kosten |
|-----------|-----------|-----------------|--------|
| DMS | Kraft, Druck | Mittel | Niedrig |
| Thermoelement | Temperatur | Niedrig | Niedrig |
| RTD (Pt100) | Temperatur | Hoch | Mittel |
| NTC | Temperatur | Hoch | Niedrig |
| Infrarot | Temperatur | Mittel | Mittel |
| MEMS-Beschleunigung | Beschleunigung | Hoch | Mittel |

---

## 5. Zusammenfassung

- **Mechanische Sensoren** wandeln Kraft, Druck und Bewegung in elektrische Signale um
- **Widerstandssensoren** nutzen Widerstandsänderungen zur Messung
- **Thermosensoren** erfassen Temperatur über verschiedene physikalische Effekte
- Die Wahl des Sensors hängt von Messgröße, Genauigkeit und Anwendungsbereich ab