# PHP Variables

Wat zijn de eerste stappen die een beginnend ontwikkelaar moet doen bij het leren van php?
Als beginnend ontwikkelaar die PHP wil leren, zijn hier enkele stappen die je zou moeten overwegen:

Leer de basisprincipes van programmeren: voordat je begint met PHP, moet je de basisprincipes van programmeren begrijpen. Leer bijvoorbeeld over variabelen, gegevenstypen, lussen en beslissingsstructuren.

Leer HTML en CSS: PHP wordt vaak gebruikt in combinatie met HTML en CSS om dynamische webpagina's te maken. Leer daarom ook de basis van HTML en CSS.

Installeer een ontwikkelomgeving: installeer een lokale serveromgeving op je computer, zoals XAMPP of WAMP, waarop je PHP-scripts kunt uitvoeren en testen.

Leer de syntax van PHP: leer de syntax van PHP door middel van online tutorials, video's en documentatie. Begin met eenvoudige concepten en ga geleidelijk verder naar complexere onderwerpen.

Schrijf code: oefen met het schrijven van eenvoudige PHP-scripts en experimenteer met de code om de resultaten te begrijpen. Begin bijvoorbeeld met het maken van een contactformulier of een inlogpagina.

Maak gebruik van de community: er zijn tal van online bronnen en forums die je kunnen helpen bij het leren van PHP. Maak gebruik van deze community om vragen te stellen en feedback te krijgen op je code.

Blijf oefenen: oefening baart kunst! Blijf oefenen en probeer steeds complexere scripts te schrijven. Zo ontwikkel je je vaardigheden en word je een betere PHP-ontwikkelaar.

## Variabelen
In PHP zijn er verschillende soorten variabelen die je kunt gebruiken om gegevens op te slaan. Hieronder volgt een overzicht van de belangrijkste variabelentypen in PHP:

* Integer: een integer is een geheel getal zonder decimalen. Bijvoorbeeld: $leeftijd = 25;
* Float: een float is een getal met decimalen. Bijvoorbeeld: $prijs = 12.50; 
* String: een string is een reeks tekens, zoals letters en cijfers, tussen aanhalingstekens. Bijvoorbeeld: $naam = "Jan Janssen"; 
* Boolean: een boolean kan alleen de waarde true of false hebben. Bijvoorbeeld: $ingeschreven = true; 
* Array: een array is een verzameling van gegevens van hetzelfde type. Bijvoorbeeld: $kleuren = array("rood", "groen", "blauw"); 
* Object: een object is een instantie van een class. Bijvoorbeeld: $auto = new Auto(); 
* NULL: NULL is een speciaal datatype dat aangeeft dat een variabele geen waarde heeft.

Naast deze typen zijn er nog enkele andere datatypen in PHP, zoals resource, callback en iterable. Door het gebruik van deze variabelentypen kun je verschillende soorten gegevens opslaan en verwerken in je PHP-code.

## integer 
Een integer in PHP is een datatypen waarmee je gehele getallen kunt opslaan en bewerken. In PHP kun je positieve en negatieve gehele getallen gebruiken als integers.

Je kunt een integer definiëren door het getal direct aan een variabele toe te wijzen. Bijvoorbeeld:

```php
$leeftijd = 30;
```
In dit voorbeeld hebben we een variabele genaamd $leeftijd gemaakt en het integerwaarde 30 eraan toegewezen.

Je kunt ook rekenkundige bewerkingen uitvoeren met integers, zoals optellen, aftrekken, vermenigvuldigen en delen. Bijvoorbeeld:

```php
$a = 10;
$b = 5;
$c = $a + $b; // $c bevat nu de waarde 15
```
In dit voorbeeld hebben we twee integers gedefinieerd, $a en $b, en deze samengevoegd met de optelling operator '+' en opgeslagen in een derde variabele genaamd $c.

In PHP kun je integers ook gebruiken in voorwaardelijke verklaringen en lussen. Bijvoorbeeld:

```php
$leeftijd = 20;

if ($leeftijd >= 18) {
  echo "Je bent volwassen";
} else {
  echo "Je bent nog geen volwassene";
}
```
In dit voorbeeld hebben we een $leeftijd variabele gedefinieerd en gecontroleerd of deze groter is dan of gelijk is aan 18. Als dit het geval is, wordt de tekst "Je bent volwassen" afgedrukt, anders "Je bent nog geen volwassene".

Dit zijn slechts enkele voorbeelden van hoe je integers in PHP kunt gebruiken. Met deze datatypen kun je eenvoudige en complexe berekeningen uitvoeren in je PHP-code.

## float 
Een float is een datatype in PHP waarmee je getallen met decimalen kunt opslaan en bewerken. Floats worden ook wel "drijvende komma" genoemd omdat de decimale punt "drijft" en de positie van de punt afhangt van het getal zelf.

Je kunt een float definiëren door het getal direct aan een variabele toe te wijzen. Bijvoorbeeld:

```php
$prijs = 12.50;
```

In dit voorbeeld hebben we een variabele genaamd $prijs gemaakt en de float-waarde 12.50 eraan toegewezen.

Je kunt ook rekenkundige bewerkingen uitvoeren met floats, zoals optellen, aftrekken, vermenigvuldigen en delen. Bijvoorbeeld:

```php
$a = 3.14;
$b = 2.5;
$c = $a * $b; // $c bevat nu de waarde 7.85
```

In dit voorbeeld hebben we twee floats gedefinieerd, $a en $b, en deze vermenigvuldigd met de vermenigvuldigingsoperator '*' en opgeslagen in een derde variabele genaamd $c.

In PHP kun je floats ook gebruiken in voorwaardelijke verklaringen en lussen. Bijvoorbeeld:

```php
$prijs = 9.99;

if ($prijs < 10.00) {
  echo "Het product is goedkoop";
} else {
  echo "Het product is duur";
}
```

In dit voorbeeld hebben we een $prijs variabele gedefinieerd en gecontroleerd of deze kleiner is dan 10.00. Als dit het geval is, wordt de tekst "Het product is goedkoop" afgedrukt, anders "Het product is duur".

Dit zijn slechts enkele voorbeelden van hoe je floats in PHP kunt gebruiken. Floats zijn een belangrijk datatype voor het werken met getallen die decimalen bevatten.




## string
Een string in PHP is een datatype dat wordt gebruikt om tekstuele gegevens op te slaan en te manipuleren. Dit kan een enkel woord, een zin, een alinea of zelfs hele pagina's tekst zijn.

Je kunt een string definiëren door tekst tussen aanhalingstekens te plaatsen en deze aan een variabele toe te wijzen. Bijvoorbeeld:

```php
$naam = "John";
```

In dit voorbeeld hebben we een variabele genaamd $naam gemaakt en de string "John" eraan toegewezen.

Je kunt ook meerdere strings samenvoegen (concateneren) met behulp van de puntoperator '.'. Bijvoorbeeld:

```php
$voornaam = "John";
$achternaam = "Doe";
$volledigeNaam = $voornaam . " " . $achternaam; // $volledigeNaam bevat nu "John Doe"
```

In dit voorbeeld hebben we twee strings gedefinieerd, $voornaam en $achternaam, en deze samengevoegd met behulp van de puntoperator en opgeslagen in een derde variabele genaamd $volledigeNaam.

In PHP kun je ook strings manipuleren met behulp van ingebouwde functies, zoals strlen() om de lengte van een string te bepalen of strpos() om de positie van een substring in een string te vinden. Bijvoorbeeld:

```php
$tekst = "Dit is een voorbeeldtekst";
$lengte = strlen($tekst); // $lengte bevat nu 24
$positie = strpos($tekst, "voorbeeld"); // $positie bevat nu 11
```

In dit voorbeeld hebben we een string genaamd $tekst gedefinieerd en de lengte bepaald met de strlen() functie en de positie van het woord "voorbeeld" gevonden met de strpos() functie.

Dit zijn slechts enkele voorbeelden van hoe je strings in PHP kunt gebruiken. Strings zijn een belangrijk datatype voor het werken met tekstuele gegevens.

## string functies van php
Er zijn veel stringfuncties in PHP. Hieronder staan enkele van de meest gebruikte functies opgesomd:

* strlen(): Geeft de lengte van een string terug. 
* str_replace(): Zoekt naar een bepaalde substring in een string en vervangt deze door een andere substring. 
* strpos(): Zoekt naar de positie van de eerste voorkomen van een substring in een string. 
* substr(): Geeft een deel van een string terug, beginnend bij de opgegeven positie en met de opgegeven lengte. 
* strtolower(): Converteert alle karakters in een string naar kleine letters. 
* strtoupper(): Converteert alle karakters in een string naar hoofdletters. 
* ucfirst(): Converteert de eerste letter van een string naar een hoofdletter. 
* ucwords(): Converteert de eerste letter van elk woord in een string naar een hoofdletter. 
* trim(): Verwijdert spaties en andere tekens vanaf het begin en het einde van een string. 
* str_repeat(): Herhaalt een string een aantal keer. 
* strrev(): Keert de volgorde van een string om. 
* implode(): Voegt de elementen van een array samen tot een string, gescheiden door een opgegeven teken. 
* explode(): Splitst een string in een array op basis van een opgegeven teken.

Dit zijn slechts enkele voorbeelden van stringfuncties die beschikbaar zijn in PHP. Er zijn nog veel meer functies die je kunt gebruiken om strings te manipuleren en te bewerken. Het is raadzaam om de officiële PHP-documentatie te raadplegen voor een volledige lijst van stringfuncties en hun beschrijvingen.

## boolean 
Een boolean in PHP is een datatype dat slechts twee waarden kan hebben: true of false. Dit wordt vaak gebruikt voor het testen van voorwaarden in code.

Je kunt een boolean definiëren door het sleutelwoord true of false aan een variabele toe te wijzen. Bijvoorbeeld:

```php
$isActief = true;
```

In dit voorbeeld hebben we een variabele $isActief gemaakt en de waarde true eraan toegewezen.

Boolean variabelen worden vaak gebruikt in combinatie met conditionele statements zoals if en while om te bepalen welke code moet worden uitgevoerd. Bijvoorbeeld:

```php
$isActief = true;

if ($isActief) {
  // voer deze code uit als $isActief true is
} else {
  // voer deze code uit als $isActief false is
}
```

In dit voorbeeld gebruiken we de $isActief variabele in een if statement om te bepalen welke code moet worden uitgevoerd. Als $isActief true is, wordt de code binnen de eerste codeblok uitgevoerd. Anders wordt de code binnen de tweede codeblok uitgevoerd.

Boolean waarden kunnen ook worden geretourneerd door vergelijkings- en logische operatoren zoals ==, !=, &&, || en !. Bijvoorbeeld:

```php
$leeftijd = 25;

$isVolwassen = ($leeftijd >= 18);

if ($isVolwassen) {
  // voer deze code uit als $leeftijd groter of gelijk is aan 18
} else {
  // voer deze code uit als $leeftijd kleiner is dan 18
}
```

In dit voorbeeld maken we gebruik van de vergelijkingsoperator >= om te testen of de waarde van $leeftijd groter of gelijk is aan 18 en slaan het resultaat op in de variabele $isVolwassen. Vervolgens gebruiken we $isVolwassen in een if statement om te bepalen welke code moet worden uitgevoerd.

Dit zijn slechts enkele voorbeelden van hoe je booleans in PHP kunt gebruiken. Booleans zijn een belangrijk datatype voor het testen van voorwaarden en het bepalen welke code moet worden uitgevoerd.

## array
Een array in PHP is een datatype dat meerdere waarden kan bevatten en deze kan groeperen onder één variabele. Een array kan bestaan uit verschillende soorten waarden zoals integer, string, float en booleans. Elke waarde in een array heeft een unieke sleutel die kan worden gebruikt om de waarde op te halen.

Een voorbeeld van het maken van een array in PHP is als volgt:

```php
$fruit = array("appel", "banaan", "peer");
```

In dit voorbeeld hebben we een array genaamd $fruit gemaakt met drie elementen: "appel", "banaan" en "peer". Om een array te definiëren, gebruiken we het sleutelwoord array gevolgd door de waarden tussen haakjes. Elke waarde in de array wordt gescheiden door een komma.

We kunnen elk element in de array ophalen door de sleutel van het element te gebruiken. De sleutels beginnen met 0 voor het eerste element, 1 voor het tweede element, enzovoort. Bijvoorbeeld:

```php
echo $fruit[0]; // geeft "appel" terug
echo $fruit[1]; // geeft "banaan" terug
echo $fruit[2]; // geeft "peer" terug
```

In dit voorbeeld gebruiken we de sleutels van de array $fruit om de waarden van elk element op te halen en ze naar het scherm te schrijven met de echo-functie.

Arrays kunnen ook worden gemaakt met sleutel-waarde paren. Bijvoorbeeld:

```php
$personen = array("Jan" => 32, "Piet" => 45, "Klaas" => 27);
```

In dit voorbeeld hebben we een array gemaakt met de naam $personen en drie sleutel-waarde paren: "Jan" met waarde 32, "Piet" met waarde 45 en "Klaas" met waarde 27. We kunnen deze waarden ophalen door de sleutel van het element te gebruiken, bijvoorbeeld:

```php
echo $personen["Jan"]; // geeft 32 terug
echo $personen["Piet"]; // geeft 45 terug
echo $personen["Klaas"]; // geeft 27 terug
```

In dit voorbeeld gebruiken we de sleutels van de array $personen om de waarden van elk element op te halen en ze naar het scherm te schrijven met de echo-functie.

Dit zijn slechts enkele voorbeelden van hoe arrays kunnen worden gemaakt en gebruikt in PHP. Arrays zijn een belangrijk datatype voor het opslaan en groeperen van meerdere waarden onder één variabele.

## object 

In PHP is een object een instantie van een klasse. Een klasse definieert de eigenschappen en methoden die een object kan hebben. Een object kan worden gezien als een container voor gegevens (eigenschappen) en functies (methoden) die ermee werken.

Hieronder staat een voorbeeld van het definiëren van een klasse en het instantiëren van een object:

```php
class Persoon {
    public $naam;
    public $leeftijd;
    
    public function groet() {
        echo "Hallo, mijn naam is " . $this->naam . " en ik ben " . $this->leeftijd . " jaar oud.";
    }
}

$persoon1 = new Persoon();
$persoon1->naam = "Jan";
$persoon1->leeftijd = 32;
$persoon1->groet(); // geeft "Hallo, mijn naam is Jan en ik ben 32 jaar oud."
```

In dit voorbeeld definiëren we een klasse genaamd Persoon. De klasse heeft twee eigenschappen: $naam en $leeftijd, en één methode: groet(). De groet()-methode gebruikt de $naam- en $leeftijd-eigenschappen om een begroeting naar het scherm te schrijven.

We maken vervolgens een nieuw object $persoon1 aan van het type Persoon. We stellen de eigenschappen $naam en $leeftijd in op "Jan" en 32, respectievelijk. We roepen vervolgens de groet()-methode aan op het $persoon1-object om de begroeting naar het scherm te schrijven.

Dit is slechts een voorbeeld van hoe objecten in PHP kunnen worden gedefinieerd en gebruikt. Objecten zijn een belangrijk concept in objectgeoriënteerd programmeren (OOP) en maken het mogelijk om complexe systemen te modelleren en efficiënter te programmeren.


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