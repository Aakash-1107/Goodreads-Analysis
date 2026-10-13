#  Goodreads Datenanalyse

##  Projektübersicht
Dieses Projekt analysiert Goodreads-Lesedaten, um Muster im Leseverhalten, Bewertungsverhalten und bei Autorenpräferenzen zu erkennen. Das Repository enthält einen anonymisierten Beispieldatensatz, und über die Umgebungsvariable `GOODREADS_CSV` kann der eigene Goodreads-Export analysiert werden (siehe Daten).

Ziel dieses Projekts ist es, Datenanalysetechniken mit Python anzuwenden und die gewonnenen Erkenntnisse klar und verständlich zu visualisieren.

---

##  Datenbereinigung & Vorbereitung
- Datumswerte in das richtige Datumsformat umgewandelt
- "Jahr" und "Monat" aus den Lesedaten extrahiert
- Fehlende Werte behandelt (z. B. Publisher → als "Self Published" markiert)
- Daten für gezielte Analysen gefiltert (z. B. Bücher aus dem Jahr 2025)

---

##  Analysen

###  Leseverhalten über die Zeit
- Anzahl gelesener Bücher pro Jahr analysiert
- 2025 als aktivstes Lesejahr identifiziert

###  Monatliche Lesemuster (2025)
- Visualisierung der Leseaktivität pro Monat
- Schwankungen und Spitzen im Leseverhalten erkannt

###  Bewertungsanalyse
- Eigene Bewertungen mit durchschnittlichen Goodreads-Bewertungen verglichen
- Ähnlichkeiten mit allgemeinen Nutzerbewertungen festgestellt

###  Autorenanalyse
- Am häufigsten gelesene Autoren identifiziert
- Präferenzen im Leseverhalten aufgezeigt

###  Verlagsanalyse
- Fehlende Verlagsdaten untersucht
- Unbekannte Einträge als "Self Published" klassifiziert

---

##  Beispiel-Visualisierungen
Die folgenden Diagramme basieren auf den anonymisierten Beispieldaten, die die ursprünglichen Anzahlen, Datumsangaben und Bewertungen beibehalten.

###  Gelesene Bücher pro Jahr
![Gelesene Bücher pro Jahr](Charts/books_per_year.png)

###  Gelesene Bücher pro Monat im Jahr 2025
![Gelesene Bücher pro Monat](Charts/Books_per_month_2025.png)

###  Verlagsverteilung
![Verlagsverteilung](Charts/Publisher_Distribution.png)

###  Bewertung vs. Durchschnittsbewertung
[Interaktive Version anzeigen](https://aakash-1107.github.io/Goodreads-Analysis/Charts/Rating_vs_Avg.html)

###  Top-Autoren
![Top-Autoren](Charts/Top_Authors_Distribution.png)

---

##  Wichtige Erkenntnisse
Diese Erkenntnisse stammen aus den anonymisierten Beispieldaten, die die ursprünglichen Anzahlen, Datumsangaben und Bewertungen beibehalten.
- Die Leseaktivität ist im Jahr 2025 deutlich gestiegen
- Das Leseverhalten variiert je nach Monat
- Eigene Bewertungen stimmen größtenteils mit Durchschnittswerten überein
- Ein Teil der Bücher ist selbst veröffentlicht
- Bestimmte Autoren werden häufiger gelesen

---

##  Technologien
- Python
- Pandas
- Matplotlib
- Seaborn
- Plotly

---
##  Daten
Das Repository enthält `Data/sample_goodreads_library.csv`, eine anonymisierte Version eines persönlichen Goodreads-Datensatzes. Buchtitel sind durch Platzhalter ersetzt ("Book 001", ...), Book Ids wurden neu nummeriert, und ISBN, ISBN13, My Review und Private Notes sind leer. Alle anderen Spalten, darunter Datumsangaben, Bewertungen, Autoren und Verlage, sind unverändert.

Um die eigene Bibliothek zu analysieren, exportiere sie aus Goodreads (My Books → Import and export → Export Library) und setze die Umgebungsvariable `GOODREADS_CSV` auf die heruntergeladene CSV-Datei. Ist `GOODREADS_CSV` nicht gesetzt, verwendet das Notebook die Beispieldaten.

---
##  Projekt ausführen

1. Repository klonen  
2. Benötigte Bibliotheken installieren:  
   `pip install -r requirements.txt`
3. (Optional) Eigenen Goodreads-Export verwenden:
   - PowerShell: `$env:GOODREADS_CSV = "C:\pfad\zu\goodreads_library_export.csv"`
   - macOS/Linux: `export GOODREADS_CSV=/pfad/zu/goodreads_library_export.csv`
4. Jupyter mit `python -m notebook` starten und anschließend `Goodreads_analysis.ipynb` öffnen

---

##  Zukünftige Verbesserungen
- Analyse nach Genres
- Entwicklung eines Empfehlungssystems
- Erweiterte statistische Analysen

---

##  Fazit
Dieses Projekt zeigt praktische Fähigkeiten in der Datenanalyse, einschließlich Datenbereinigung, Visualisierung und Interpretation von Ergebnissen. Es demonstriert, wie persönliche Daten genutzt werden können, um aussagekräftige Erkenntnisse zu gewinnen.
