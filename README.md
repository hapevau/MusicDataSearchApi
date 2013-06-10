# Erster Teil der API-Sourcen

API zum Zugriff auf die wichtigsten API's für Musikdateien.

- Wikipedia (deutsch und englisch)
- musibrainz
- discogs

Das Projekt ist folgendermassen strukturiert:

- in base liegen die Basisklassen für Links und Ergebnisparser
- in search liegen konkrete Instanzen für obige API-Provider und eine Request-Kollektion zur Verwendung.

In der Indexdatei (index.js) ist die Verwendung der API gezeigt.
Man setzt den Suchbegriff (entweder für alle Provider oder einen speziellen) und ruft dann die Methode makeRequest auf, der
man eine callback-Funktion mitgibt.

Die API kann jetzt schon für Artisten/Gruppen-Suche verwendet werden - wird aber weiter entwickelt, um anhand der gefunden 
IDs die Musikdaten dann abzurufen.

Anhand der Basisklasen in Base können eigene Linktypen und Parser einfach entwickelt werden und in der API verwendet.

Die Dokumentation der verwendeten Provider ist auf meinem Blog http://hpv.leo.uberspace.de zu finden
