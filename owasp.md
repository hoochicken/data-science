# OWASP

## Rollen/Ansichten:

* Leser
* News-Einsteller +  Display
* yii-Verwaltung
* Release-News-Vorschau

## C4 model for visualizing

* verschiedene zoom-Levels (4) 
    * Context 
		* Flughöhe 20 km
		* grobe Darstellung
		* System im Fokus, grob
	* Container (Applikationen, Service)
		* Flughöhe 5 km
		* detailliertere Darstellung
		* System im Fokus, detailliert
		* REST, Schnittstelle, Rollen, Datenbank, 
	* Component () 
		* Flughöhe 1 km
		* Detail einer Komponente
		* Controller, SiteController, Service-Klasse
	* Code -> UML
* In Kommunktation mit Support sind eigentlich nur die ersten 3 Levle von Beland

## Plant UML

* pUML-Datei
* generiert eine passende Grafik 
* Plugin für PhpStorm

## yii-App

* bestimmte Teile im Code markiert, wird automatisch durch AJAX nachgeladen
* CKEditor eingebunden
* Mehrsprachigkeits-Komponente
* Soft-Deletes

## Randbemerkungen

* Rapid Application Development (RAD)
* "monolit" mit modulen (umbrella app docker elexir phoenix) vs. repo-sammlung
* Release-News ist damit ein klassischer Microservice, der sich nur um EINE Sache kümmert
* ein Repo für 4 Unterprodukte, z. T. mit Quick-and-dirty-Lösungen
* Arbeitsweise / Teamgrösse ist mit entscheidend für die Architektur-Wahl

## Review

* würde TB wieder so umsetzen
* Portierung in andere Programmiersprachen schwierig (Proxy in Php sind z. T. träge, also ggf. wäre eine andere Sprache)
* Abgrenzungsfrage: wo ziehe ich Grenzen meiner Applikation?
* Tests? Technische Schuld, Unit-Tests, API-Test, GUI-Test?
