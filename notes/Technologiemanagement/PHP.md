## Grundlagen

PHP ist eine serverseitige Skriptsprache für Webentwicklung. PHP-Code wird in HTML eingebettet und auf dem Server ausgeführt.

```php
<?php echo "Hallo, Welt!"; ?>
```

## Variablen und Datentypen

```php
$text = "Hallo"; 
$zahl = 42; 
$kommazahl = 3.14; 
$wahrheitswert = true; 
$array = ["Apfel", "Banane", "Kirsche"];
```

## Kontrollstrukturen

```php
if ($bedingung) {
	// Code 
} elseif ($andere_bedingung) {    
	// Code 
} else {     
	// Code 
} 
for ($i = 0; $i < 10; $i++) {     
	// Code 
} while ($bedingung)  {     
	// Code 
} foreach ($array as $wert) {     
	// Code 
}
```

## Funktionen

```php
function begrüßung($name) {     
	return "Hallo, $name!"; 
}

echo begrüßung("Welt");
```

## Arrays

```php
$früchte = ["Apfel", "Banane", "Kirsche"]; 
echo $früchte[0]; // Gibt aus: Apfel 
$person = [ "name" => "Hans", "alter" => 30 ]; 
echo $person["name"]; // Gibt aus: Hans
```

## Klassen und Objekte

```php
class Person {     
	public $name;    
	public $alter;     
	public function __construct($name, $alter) {        
	$this->name = $name;        
	$this->alter = $alter;    
	}     
	public function vorstellen() {        
		echo "Ich bin {$this->name} und {$this->alter} Jahre alt.";    
	} 
} 
$hans = new Person("Hans", 30); $hans->vorstellen();
```

## Datenbankoperationen (MySQL-Beispiel)

```php
$verbindung = mysqli_connect("host", "benutzername", "passwort", "datenbank"); $ergebnis = mysqli_query($verbindung, "SELECT * FROM benutzer"); 
while ($zeile = mysqli_fetch_assoc($ergebnis)) {     
	echo $zeile["name"]; 
}
```

## Fehlerbehandlung

```php
try {     
	// Code, der eine Ausnahme werfen könnte 
} catch (Exception $e) {     
	echo "Fehler: " . $e->getMessage(); 
} finally {     // Wird immer ausgeführt 
}
```

## Superglobale Variablen

```php
echo $_GET['parameter'];  // URL-Parameter 
echo $_POST['feld'];      // Formulardaten 
echo $_SESSION['user'];   // Sitzungsdaten 
echo $_COOKIE['präferenz']; // Cookie-Daten`
```
## Namensräume

```php
namespace MeinProjekt\Util; 

class Helfer {     
	// Klasseninhalt 
} 

use MeinProjekt\Util\Helfer; 

$helfer = new Helfer();
```

## Traits

```php
trait LoggerTrait {     
	public function log($nachricht) {        
		echo "Protokoll: $nachricht";    
	} 
} 
class MeineKlasse {     
	use LoggerTrait; 
} 

$objekt = new MeineKlasse(); $objekt->log("Hallo");`