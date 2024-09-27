HTML (Hypertext Markup Language) ist die Standard-Auszeichnungssprache zur Erstellung von Webseiten. Es verwendet eine Reihe von Elementen (Tags), um Inhalte im Internet zu strukturieren und darzustellen. ### 1. **Grundstruktur eines HTML-Dokuments** Ein HTML-Dokument beginnt typischerweise mit einer `<!DOCTYPE html>`-Deklaration, gefolgt vom `<html>`-Element, das die Bereiche `<head>` und `<body>` enthält. 

```html 
<!DOCTYPE html> 
<html lang="de"> 
	<head> 
		<meta charset="UTF-8"> 
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>Titel des Dokuments</title> 
	</head> 
	<body> 
		<h1>Hallo, Welt!</h1> 
		<p>Dies ist eine grundlegende HTML-Seitenstruktur.</p> 
	</body> 
</html>
```
___
### Häufige HTML-Elemente

**Überschriften**: Werden verwendet, um Überschriften zu definieren. `<h1>` ist die höchste Ebene, und `<h6>` ist die niedrigste.

```html
<h1>Hauptüberschrift</h1> 
<h2>Unterüberschrift</h2> 
<h3>Abschnittsüberschrift</h3>
```

**Absätze**: Repräsentieren Textblöcke.

```html
<p>Dies ist ein Absatz mit Text.</p>
```

**Links**: Erstellen Hyperlinks mit dem `<a>`-Tag.

```html
<a href="https://www.beispiel.de">Beispiel besuchen</a>
```

**Bilder**: Zeigen Bilder mit dem `<img>`-Tag an.

```html
<img src="bild.jpg" alt="Beschreibung des Bildes">
```

**Geordnete Liste**: Nummerierte Liste

```html
<ol> <li>Erster Punkt</li> <li>Zweiter Punkt</li> </ol>
```

**Ungeordnete Liste**: Aufzählungspunkte

```html
<ul> <li>Erster Punkt</li> <li>Zweiter Punkt</li> </ul>
```

### Attribute

Attribute liefern zusätzliche Informationen über Elemente. Sie werden immer im Öffnungstag enthalten und als Name/Wert-Paare wie `name="wert"` geschrieben.

```html
<a href="https://www.beispiel.de" target="_blank">In neuem Tab öffnen</a> 
<img src="bild.jpg" alt="Eine schöne Landschaft" width="500">
```

### Formulare

Formulare ermöglichen es Benutzern, Daten an einen Server zu senden.

```html
<form action="/absenden" method="post"> 
	<label for="name">Name:</label> 
	<input type="text" id="name" name="name"> 
	<button type="submit">Absenden</button> 
</form>
```

### Tabellen

Tabellen organisieren Daten in Zeilen und Spalten.

```html
<table> 
	<tr> 
		<th>Name</th> 
			<th>Alter</th> 
		</tr> 
	<tr> 
		<td>Max</td> 
		<td>30</td> 
	</tr> 
	<tr> 
		<td>Anna</td> 
		<td>25</td> 
	</tr> 
</table>
```

