#PHP Variables

## array
Een array in PHP is een geordende lijst van elementen die zijn geïndexeerd met numerieke sleutels. Elk element in een array heeft een unieke sleutel waarmee het kan worden geïdentificeerd. De sleutels van een array kunnen numeriek of alfanumeriek zijn. In PHP kunnen arrays ook associatief zijn, wat betekent dat de elementen worden geïndexeerd met tekstuele sleutels in plaats van numerieke sleutels.

De syntax om een array in PHP te maken is als volgt:

```php

$naam_van_array = [element1, element2, element3, ...];
```


Hier is een voorbeeld van een numerieke array in PHP die drie strings bevat:

```php
$kleuren = ['rood', 'groen', 'blauw'];
of
$kleuren = array('rood', 'groen', 'blauw');
```
In dit voorbeeld hebben we een array genaamd $kleuren gemaakt met drie elementen: 'rood', 'groen' en 'blauw'. We kunnen de elementen van de array opvragen door hun sleutels (0, 1, 2) te gebruiken:

```php
echo $kleuren[0]; // geeft 'rood' terug
echo $kleuren[1]; // geeft 'groen' terug
echo $kleuren[2]; // geeft 'blauw' terug
```
We kunnen ook een associatieve array maken in PHP door tekstuele sleutels te gebruiken in plaats van numerieke sleutels. Hier is een voorbeeld van een associatieve array in PHP die informatie over een persoon bevat:

```php
$persoon = [
    'naam' => "Jan",
    'leeftijd' => 30,
    'beroep' => "leraar"
];
```
In dit voorbeeld hebben we een array genaamd $persoon gemaakt met drie elementen, die elk zijn geïndexeerd met een tekstuele sleutel. We kunnen de elementen van de array opvragen door hun sleutels te gebruiken:

```php
echo $persoon["naam"];     // geeft "Jan" terug
echo $persoon["leeftijd"]; // geeft 30 terug
echo $persoon["beroep"];   // geeft "leraar" terug
```
Arrays zijn een krachtig hulpmiddel in PHP omdat ze ons in staat stellen om gegevens op een gestructureerde manier op te slaan en te manipuleren. We kunnen arrays gebruiken om lijsten van items, tabelgegevens en associatieve gegevens op te slaan en te beheren.

# Loops
## foreach loop

Een foreach loop in PHP is een type loop dat is ontworpen om gemakkelijk te itereren over elementen in een array of object. De syntax van een foreach loop in PHP is als volgt:
```php
foreach ($array as $value) {
    // code om te herhalen
}
```
* $array: De array die je wilt doorlopen met de foreach loop.
* $value: Een tijdelijke variabele die de huidige waarde van het element in de array bevat.

Hier is een voorbeeld van een foreach loop in PHP die de waarden van een array afdrukt:
```php
<?php
$colors = ["rood", "groen", "blauw"];
foreach ($colors as $color) {
    echo $color . " ";
}
?>
```

In dit voorbeeld wordt de foreach loop gebruikt om door de $colors array te itereren en de waarde van elk element af te drukken met behulp van echo. De variabele $color bevat de waarde van het huidige element in de array tijdens elke iteratie van de lus. Het resultaat van dit script is:

```php
rood groen blauw
````
U kunt ook de sleutels en waarden van een associatieve array afzonderlijk doorlopen met behulp van de foreach loop. Hier is een voorbeeld:

```php
<?php
$person = ['naam' => "Jan", 'leeftijd' => 30, 'beroep"=> "leraar"];
foreach ($person as $key => $value) {
    echo $key . ": " . $value . "<br>";
}
?>
```
In dit voorbeeld wordt de foreach loop gebruikt om door de $person associatieve array te itereren en de sleutels en waarden van elk element af te drukken met behulp van echo. De variabele $key bevat de sleutel van het huidige element in de array en $value bevat de waarde ervan. Het resultaat van dit script is:

```php
naam: Jan
leeftijd: 30
beroep: leraar
```
<hr>

## for loop
Een for loop in PHP is een type loop waarbij een variabele wordt geïnitialiseerd, een voorwaarde wordt getest en een incrementerende of decrementerende stap wordt uitgevoerd totdat de voorwaarde niet meer waar is. De syntax van een for loop in PHP is als volgt:
```php

for (init; test; increment) {
    // code om te herhalen
}
```
* init: Een expressie die wordt uitgevoerd aan het begin van de lus en die de lusvariabele initialiseert.
* test: Een expressie die aan het begin van elke lusiteratie wordt geëvalueerd en die bepaalt of de lus doorgaat of stopt.
* increment: Een expressie die aan het einde van elke lusiteratie wordt uitgevoerd en de lusvariabele verhoogt of verlaagt.

Hier is een voorbeeld van een for loop in PHP die de getallen 1 tot en met 10 afdrukt:
```php

<?php
for ($i = 1; $i <= 10; $i++) {
    echo $i . " ";
}
?>
```

In dit voorbeeld wordt de variabele $i geïnitialiseerd met de waarde 1. Vervolgens wordt de test uitgevoerd om te controleren of $i kleiner of gelijk is aan 10. Omdat dit waar is, wordt de code in de lus uitgevoerd en wordt $i afgedrukt met behulp van echo. Daarna wordt $i verhoogd met 1. Dit proces herhaalt zich totdat $i niet langer kleiner of gelijk is aan 10, waarna de lus stopt en de uitvoering van de rest van het script doorgaat.