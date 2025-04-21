# lebensmittelpreise-bigdata
Analyse von Lebensmittelpreisen in österreichischen Supermärkten

Dieses Projekt untersucht Preisentwicklungen und Unterschiede von Produkten in verschiedenen Supermarktketten (z. B. Billa, Spar) mithilfe moderner Big Data Infrastruktur.

## Projektstruktur
- `/data` – CSV-Dateien und Rohdaten
- `/scraper` – Python-Skripte für Web Scraping
- `/notebooks` – Jupyter Notebooks für Analyse & Visualisierung
- `/docker` – Docker-Konfigurationen (MongoDB etc.)

## vorläufige Team & Aufgabenverteilung 
## Pinar: (Scraping & Datenbeschaffung)
- Zielseiten analysieren (z. B. HTML-Struktur von Billa, Spar)
- Web Scraper mit Python schreiben (inkl. Test-URLs)
- Testdatensätze im CSV-Format erstellen

## Ambar (Analyse vorbereiten)
- Jupyter Notebook mit Gliederung & Beispielcode vorbereiten
- Pandas-Logik mit fiktiven Daten testen (z. B. preise_test.csv)
- MapReduce-Logik unabhängig vom echten Datensatz erstellen

## Julia (Doku & Visualisierung)
- README.md schreiben (Projektbeschreibung + Rollen)
- Architekturdiagramm zeichnen (z. B. mit draw.io)
- Präsentation (Folienstruktur) vorbereiten
- Erste Dummy-Plots mit z. B. {"Milch": 1.29, "Brot": 2.49}

## Technologien
Python, Pandas, MongoDB, MapReduce, Docker, GitHub

## Datenquellen
- **Supermarkt-Websites** (Billa, Spar, Hofer)  
  → Scraping von Online-Preisen für Produkte wie Milch, Brot, Eier

- **Statistik Austria / Open Data Österreich**  
  → Nutzung öffentlich zugänglicher Preisstatistiken für Lebensmittel (z. B. Verbraucherpreisindex)

- **Eurostat – HICP Food Price Dashboard**  
  → Vergleich von Lebensmittelpreisen auf europäischer Ebene auf Basis des harmonisierten Verbraucherpreisindex (HICP)


## Big Data Kriterien
- Volume: viele Preise aus verschiedenen Filialen
- Velocity: regelmäßig neue Daten möglich
- Variety: HTML, CSV
- Veracity: durch Websitevergleich
- Value: Erkenntnisse für Konsumenten

## 4 Ebenen der Datenverarbeitung

1. **Data Source**  
   - Supermarkt-Webseiten (Scraping)  
   - Statistik Austria / Open Data  
   - Eurostat  

2. **Data Storage**  
   - MongoDB (via Docker, NoSQL)  
   - CSV-Dateien für Zwischen- und Testdaten  

3. **Data Analysis**  
   - Pandas für Datenbereinigung & Visualisierung  
   - MapReduce für Preisentwicklungsanalyse  

4. **Data Output**  
   - Visualisierungen (Balkendiagramme etc.)  
   - Dokumentation im Jupyter Notebook  
   - Präsentation mit zentralen Ergebnissen
# lebensmittelpreise-bigdata
