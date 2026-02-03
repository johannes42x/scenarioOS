scenarioOS – Nutzungs- & Workflow-Guide

Dieses Dokument beschreibt den praktischen Workflow für die Nutzung von scenarioOS.
Es ist dafür gedacht, direkt im scenarioOS-Ordner zu liegen, und setzt keinerlei Vorkenntnisse zu MetaMemoryWorks voraus.

---

## Was scenarioOS tut

scenarioOS ermöglicht es, den *Arbeitszustand* einer langen oder komplexen Unterhaltung in eine portable Datei zu exportieren und die Arbeit später in einer neuen Session oder sogar in einem anderen Sprachmodell fortzusetzen.

Es speichert **nicht** den vollständigen Chatverlauf.
Es speichert das, was für die Fortsetzung relevant ist.

---

## Typischer Anwendungsfall

Du arbeitest in einer längeren Session:

- Ideen sammeln sich an
- Annahmen werden etabliert
- Constraints und Entscheidungen entstehen
- Tonfall und Arbeitsstil stabilisieren sich

Mit der Zeit wird die Session langsam, unübersichtlich oder fragil.
Du willst nicht neu anfangen, weil dabei zu viel impliziter Zustand verloren ginge.

Genau für diesen Moment ist scenarioOS gedacht.

---

## Grundlegender Workflow

### 1. Normal arbeiten

Starte eine Unterhaltung und arbeite ganz normal.
Du musst nichts „vorbereiten“, um scenarioOS zu nutzen.

scenarioOS erfordert während der Session kein spezielles Prompting.

---

### 2. Szenario-Export auslösen

Wenn du den aktuellen Arbeitszustand sichern möchtest, tue eines der folgenden Dinge:

- Lade die scenarioOS-Engine-Datei hoch
- Bitte das Modell, aus der aktuellen Session ein Szenario zu erzeugen

Typische Formulierungen sind zum Beispiel:
- „Exportiere das aktuelle Szenario.“
- „Erstelle einen scenarioOS-State zur Fortsetzung.“
- „Bewahre den Arbeitszustand als Szenario.“

Das Modell analysiert die Session und erzeugt eine **Szenario-Datei**.

---

### 3. Szenario-Datei speichern

Die Szenario-Datei ist die portable Repräsentation deines Arbeitszustands.

- Lade sie herunter
- Bewahre sie unverändert auf (sie ist menschenlesbar)
- Bearbeite sie nur, wenn du genau weißt, was du tust

Diese Datei ist das *Einzige*, was scenarioOS für die Fortsetzung benötigt.

---

### 4. Neue Session starten

Öffne eine neue Session – im selben oder in einem anderen LLM.

Lade die Szenario-Datei hoch.

Nutze eine minimale Anweisung wie:
- „Setze die Arbeit aus diesem Szenario fort.“
- „Fahre mit diesem Szenario fort.“
- „Orientiere dich anhand des Szenarios und arbeite weiter.“

Du musst Ziele, Tonfall oder Constraints **nicht** erneut erklären.

---

### 5. Weiterarbeiten

Das Modell sollte:

- Annahmen und Entscheidungen aufgreifen
- Constraints respektieren
- den etablierten Arbeitsstil beibehalten
- die Aufgabe kohärent fortführen

Das ist Fortsetzung, kein Replay.

---

## Modellübergreifende Nutzung

scenarioOS ist modellagnostisch.

Eine in einem Modell erzeugte Szenario-Datei kann in einem anderen Modell verwendet werden, solange Datei-Kontext unterstützt wird.

Die genaue Formulierung kann leicht variieren, der Arbeitszustand sollte sich jedoch übertragen lassen.

---

## Wann ein neues Szenario erzeugen?

Erstelle ein neues Szenario, wenn:

- die Session langsam oder instabil wird
- die Aufgabe in eine neue Phase übergeht
- du einen sauberen Checkpoint möchtest
- du das Modell oder die Umgebung wechseln willst

scenarioOS ist nicht dafür gedacht, dauerhaft im Hintergrund zu laufen.
Es markiert **Übergänge**.

---

## Was scenarioOS nicht tut

scenarioOS:

- speichert keine Erinnerungen automatisch
- verfolgt keine Nutzer über Sessions hinweg
- personalisiert Modelle nicht
- verwaltet keine Agents oder Tools
- ersetzt keine Urteils- oder Entscheidungsfindung

Es ist ein Kontinuitätsmechanismus, kein Automatisierungssystem.

---

## Best Practices

- Behandle Szenario-Dateien wie Checkpoints
- Überschreibe alte Szenarien nicht, sondern behalte sie
- Benenne Szenario-Dateien aussagekräftig
- Nutze beim Fortsetzen minimale Prompts
- Lass das Szenario die Arbeit machen

---

## Kurz gesagt

Arbeiten → Szenario exportieren → Neue Session → Weiterarbeiten.

Das ist das gesamte System.
