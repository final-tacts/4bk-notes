**Power BI** ist eine Business-Analytics-Lösung von Microsoft, die Benutzern ermöglicht, Daten zu visualisieren, interaktive Berichte zu erstellen und Geschäftsentscheidungen auf Grundlage von Daten zu treffen. Es bietet Werkzeuge zur Verbindung mit verschiedenen Datenquellen, zur Modellierung der Daten und zur Erstellung interaktiver Dashboards und Berichte.

## Warum Power BI?

1. **Visuelle Analysen**: Power BI bietet leistungsstarke Visualisierungstools, mit denen Benutzer Daten in ansprechenden Dashboards und Berichten darstellen können.
2. **Einfach zu verwenden**: Mit seiner benutzerfreundlichen Oberfläche können auch weniger erfahrene Benutzer Berichte erstellen, Daten modellieren und analysieren.
3. **Vielfältige Datenquellen**: Power BI kann Daten aus verschiedenen Quellen integrieren, darunter Datenbanken (SQL, Access), Excel, Web-APIs und viele andere.
4. **Automatische Aktualisierungen**: Berichte und Dashboards können so eingestellt werden, dass sie in regelmäßigen Abständen automatisch aktualisiert werden.
5. **Teilen und Zusammenarbeiten**: Berichte können in der Cloud veröffentlicht und leicht mit Kollegen geteilt werden.
## Kernkomponenten von Power BI

1. **Power BI Desktop**: Ein Windows-Anwendungstool zum Erstellen von Berichten und Dashboards.
2. **Power BI Service**: Ein cloudbasierter Dienst zum Teilen von Berichten und Dashboards.
3. **Power BI Mobile**: Mobile Apps, um Berichte und Dashboards unterwegs anzuzeigen.

## Grundlegender Arbeitsablauf

1. **Datenquelle verbinden**: Power BI unterstützt Verbindungen zu vielen verschiedenen Datenquellen.
2. **Daten aufbereiten und transformieren**: Mit dem Power Query Editor können Daten bereinigt und transformiert werden.
3. **Datenmodell erstellen**: Beziehungen zwischen Tabellen werden definiert, und die Daten werden strukturiert.
4. **Visualisierungen erstellen**: Mit Diagrammen, Karten, Tabellen und anderen visuellen Elementen lassen sich die Daten anschaulich darstellen.
5. **Berichte und Dashboards teilen**: Berichte können im Power BI Service veröffentlicht und mit anderen geteilt werden.

## Was ist DAX?

**DAX** (Data Analysis Expressions) ist die Formelsprache, die in Power BI, Power Pivot und SSAS verwendet wird. Sie wird verwendet, um Berechnungen und Datenmanipulationen in den Datenmodellen durchzuführen. DAX ähnelt Excel-Formeln, bietet aber zusätzliche Funktionen, die speziell für die Arbeit mit relationalen Daten und umfangreichen Datenmodellen entwickelt wurden.

### Warum DAX?

1. **Erweiterte Berechnungen**: DAX erlaubt es, berechnete Felder (Measures) zu erstellen, die komplexe Berechnungen auf Daten anwenden.
2. **Zeitintelligenz**: DAX enthält spezielle Funktionen, um Zeitreihenanalysen wie kumulierte Werte oder Jahresvergleiche durchzuführen.
3. **Filter- und Kontextfunktionen**: DAX bietet leistungsstarke Filtermöglichkeiten, um Berechnungen basierend auf bestimmten Bedingungen durchzuführen.
___
## Wichtige DAX-Funktionen

### 1. **SUM()**

Addiert alle Werte in einer bestimmten Spalte.

`SUM('Sales'[Revenue])`

### 2. **CALCULATE()**

Berechnet einen Ausdruck in einem geänderten Filterkontext. Dies ist eine der wichtigsten DAX-Funktionen.

`CALCULATE(SUM('Sales'[Revenue]), 'Sales'[Region] = "West")`

### 3. **RELATED()**

Greift auf eine verwandte Tabelle zu und gibt den entsprechenden Wert aus.

`RELATED('Customer'[CustomerName])`

### 4. **IF()**

Führt eine bedingte Prüfung durch.

`IF('Sales'[Revenue] > 1000, "High", "Low")`

### 5. **ALL()**

Ignoriert alle Filter auf eine bestimmte Spalte oder Tabelle und liefert alle Daten zurück.

`CALCULATE(SUM('Sales'[Revenue]), ALL('Sales'[Region]))`

### 6. **TIMEINTELLIGENCE-FUNKTIONEN**

Diese Funktionen helfen bei der Arbeit mit Datumswerten, um Zeitreihenanalysen durchzuführen.

- **TOTALYTD()**: Berechnet den kumulierten Gesamtwert bis zum Jahresende.
    
    `TOTALYTD(SUM('Sales'[Revenue]), 'Calendar'[Date])`
    
- **SAMEPERIODLASTYEAR()**: Vergleicht den gleichen Zeitraum im Vorjahr.
    
    `SAMEPERIODLASTYEAR('Calendar'[Date])`
    

## Beispiel für ein DAX Measure

Ein Measure ist eine dynamische Berechnung, die in einem Power BI-Bericht verwendet wird. Hier ist ein Beispiel für ein einfaches Measure, das den Gesamtumsatz berechnet:

`Total Revenue = SUM('Sales'[Revenue])`

Wenn wir den Gesamtumsatz für das Jahr berechnen möchten, könnten wir ein Measure erstellen, das die Zeitintelligenz-Funktion **TOTALYTD()** verwendet:

`Total YTD Revenue = TOTALYTD(SUM('Sales'[Revenue]), 'Calendar'[Date])`
___
## Fazit

Power BI ist ein mächtiges Tool für die Datenvisualisierung und -analyse. Mit Hilfe von DAX kannst du komplexe Berechnungen auf deine Daten anwenden und tiefere Einblicke gewinnen. Während die Benutzeroberfläche von Power BI recht intuitiv ist, ermöglicht DAX die Erstellung maßgeschneiderter Analysen, die weit über einfache Summen und Durchschnitte hinausgehen.