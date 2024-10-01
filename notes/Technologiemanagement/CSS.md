#### 1.1 Was ist CSS?
- CSS wird verwendet, um das Aussehen einer Webseite zu steuern.
- Es ist von HTML getrennt und soll Inhalt und Präsentation auseinanderhalten.
- Das **Cascade-Prinzip** in CSS bezieht sich auf die Hierarchie, in der Stile angewendet werden, wobei die spezifischste Regel Priorität hat.

#### 1.2 Wie funktioniert CSS?
- **Selektoren**: Die Elemente, die du stylen möchtest.
    - Arten von Selektoren: Element-, Klassen-, ID-, Attribut-, Pseudo-Klassen- und Pseudo-Element-Selektoren.
- **Eigenschaften und Werte**: CSS-Regeln bestehen aus Eigenschaften (wie `color`, `font-size`) und Werten (wie `red`, `16px`).

```css
h1 { 
	color: blue; 
	font-size: 24px; 
}
```

In diesem Beispiel:
- `h1` ist der Selektor.
- `color` und `font-size` sind Eigenschaften.
- `blue` und `24px` sind Werte.

#### 1.3 Möglichkeiten, CSS anzuwenden
- **Inline-CSS**: Innerhalb des HTML-Elements mit dem `style`-Attribut.

```css
<p style="color: red;">Das ist ein roter Absatz.</p>
```

* **Internes CSS**: Innerhalb eines `<style>`-Tags im `<head>` des HTML-Dokuments.

```css
<head> 
	<style> 
	p { 
		color: green; 
	} 
	</style> 
</head>
```

* **Externes CSS**: In einer separaten CSS-Datei, die mit dem HTML-Dokument verknüpft ist.

```css
<link rel="stylesheet" type="text/css" href="styles.css">
```

___
#### 2.1 Das Box-Modell

Das CSS-Boxmodell definiert, wie die Elemente auf einer Webseite strukturiert sind. Jedes Element wird als Box betrachtet, und das Boxmodell besteht aus vier Teilen:
- **Inhalt**: Der eigentliche Inhalt innerhalb der Box (Text, Bilder).
- **Innenabstand (Padding)**: Raum zwischen dem Inhalt und dem Rand.
- **Rand (Border)**: Eine Linie, die das Padding umgibt (optional).
- **Außenabstand (Margin)**: Raum zwischen dem Rand und benachbarten Elementen.

```css
div { margin: 20px; padding: 10px; border: 2px solid black; }
```

#### 2.2 Anzeigeeigenschaften

Die Eigenschaft `display` steuert das Layout von Elementen.
- **block**: Nimmt die volle Breite ein (wie `<div>`, `<p>`, `<h1>`).
- **inline**: Beginnt nicht auf einer neuen Zeile, nimmt nur so viel Platz ein, wie benötigt (wie `<span>`, `<a>`).
- **inline-block**: Verhält sich wie inline, kann aber eine Breite und Höhe haben.

```css
span { display: inline-block; width: 100px; height: 50px; }
```
#### 2.3 Positionierung

CSS bietet verschiedene Möglichkeiten, Elemente auf einer Seite zu positionieren:
- **static**: Standardpositionierung.
- **relative**: Relativ zu ihrer normalen Position.
- **absolute**: Positioniert relativ zum nächstgelegenen positionierten Vorfahren.
- **fixed**: Positioniert relativ zum Browserfenster.
- **sticky**: Eine Mischung aus `relative` und `fixed`.

```css
div { position: absolute; top: 50px; left: 100px; }
```

___
#### 3.1 Schrift-Eigenschaften

- `font-family`: Definiert die Schriftart.
- `font-size`: Steuert die Schriftgröße.
- `font-weight`: Legt die Dicke der Schrift fest (normal, fett).
- `font-style`: Kursiv oder normal.
- `line-height`: Steuert den Abstand zwischen Textzeilen.

```css
p { 
	font-family: 'Arial', sans-serif; 
	font-size: 18px; 
	font-weight: bold; 
	font-style: italic; 
}
```

#### 3.2 Texteigenschaften

- `color`: Definiert die Farbe des Textes.
- `text-align`: Richtet den Text links, rechts, zentriert oder im Blocksatz aus.
- `text-decoration`: Fügt Unterstreichungen, Überstriche oder Durchstreichungen hinzu.
- `letter-spacing`: Steuert den Abstand zwischen Buchstaben.
- `text-transform`: Konvertiert Text in Großbuchstaben, Kleinbuchstaben oder Kapitalisierungen.

```css
h2 { 
	text-align: center; 
	text-transform: uppercase; 
	letter-spacing: 2px; 
}
```

___
#### 4.1 Flexbox

Flexbox ist ein leistungsstarkes Layoutmodul zum Ausrichten und Verteilen von Elementen in einem Container, auch wenn deren Größe unbekannt ist.

- **display: flex**: Macht den Container zu einem Flex-Container.
- **flex-direction**: Steuert die Ausrichtung der Flex-Elemente (Zeile oder Spalte).
- **justify-content**: Richtet Elemente entlang der Hauptachse aus (links, rechts, zentriert).
- **align-items**: Richtet Elemente entlang der Querachse aus.

```css
.container { 
	display: flex; 
	justify-content: space-between; 
	align-items: center; 
}
```

#### 4.2 CSS Grid

CSS Grid ist ein weiteres leistungsstarkes Werkzeug, um komplexe Layouts zu erstellen. Es ermöglicht das Definieren von Zeilen und Spalten und das Platzieren von Elementen entsprechend.

- **display: grid**: Macht den Container zu einem Raster.
- **grid-template-columns**: Definiert die Spalten.
- **grid-template-rows**: Definiert die Zeilen.
- **grid-gap**: Definiert den Abstand zwischen den Rasterelementen.

```css
.container { 
	display: grid; 
	grid-template-columns: repeat(3, 1fr); 
	grid-gap: 20px; 
}
```

#### 4.3 Medienabfragen

Medienabfragen werden verwendet, um responsive Designs zu erstellen, die sich an verschiedene Bildschirmgrößen anpassen.

```css
@media (max-width: 600px) { 
	.container { 
		flex-direction: column; 
	} 
}
```

___
#### 5.1 Übergänge

CSS-Übergänge ermöglichen das sanfte Ändern von Eigenschaftswerten über eine bestimmte Dauer.

```css
button { 
	background-color: blue; 
	transition: background-color 0.3s ease; 
} 
button:hover { 
	background-color: red; 
}
```

#### 5.2 Animationen

CSS-Animationen ermöglichen komplexere, auf Keyframes basierende Animationen.

```css
@keyframes fadeIn { 
	from { 
		opacity: 0; 
	} 
	to { 
		opacity: 1; 
	} 
} 
div { 
	animation: fadeIn 2s; 
}
```

___
#### 6.1 Best Practices

- **Externe Stylesheets verwenden**: Halte Stile getrennt vom HTML.
- **Vermeide Inline-Stile**: Diese machen den Code schwer wartbar.
- **Verwende semantische HTML-Elemente**: Stelle sicher, dass CSS logisch auf die entsprechenden Elemente angewendet wird.
- **Minimiere das Über-Spezifizieren von Selektoren**: Zu spezifische Selektoren machen CSS schwer überschreibbar.

#### 6.2 Beliebte CSS-Frameworks

Frameworks können die Entwicklung beschleunigen:
- **Bootstrap**: Beliebt für responsive Designs.
- **Tailwind CSS**: Utility-First CSS-Framework.
- **Foundation**: Responsives Front-End-Framework.

___
#### 7.1 Einführung in CSS-Präprozessoren

Präprozessoren wie **SASS** und **LESS** machen CSS leistungsfähiger und wartbarer.
- Variablen
- Verschachtelung
- Mixins

Beispiel mit SASS:
```css
$primary-color: blue; 
button { 
	background-color: $primary-color; 
	&:hover { 
		background-color: darken($primary-color, 10%); 
	} 
}
```


