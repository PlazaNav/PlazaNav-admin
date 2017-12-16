# Rekapitulation der SA PlazaRoute

## Was wurde erreicht?

* Aufarbeitung der Theorie
  * Problemstellung des Fussgänger-Routings wurden unter die Lupe genommen und für mögliche Folgeprojekte aufbereitet
  * Einlesen, Evaluation durchführen, QGIS Tests schreiben, Algorithmen mit Probanden getestet
* Aufbereitung von OSM-Daten
 * SpiderWeb-Graph und Visibility-Graph können in Kombination mit einem Dijkstra oder A* für die Vorverarbeitung verwendet werden
 * "schnelle" und "kompakte" Verarbeitung der Daten
 * flexible Lösungen, welche einfach erweiterbar ist durch Konfigurationsmöglichkeiten
* multimodales Routing
  * Fussgänger-Routing in Kombination mit dem ÖV-Routing von jedem Startpunkt aussagekr
  * Visualisierung in QGIS-Plugin
* Optimierung der Genauigkeit der Koordinaten von ÖV-Haltestellen mit Overpass
  * sind die OSM-Daten von einigermassen guter Qualität, kann die Haltestelle-Kante genau angesteuert werden
  * kann gut in ein Folgeprojekt überführt werden, welches search. ch Nutzen kann, um bessere Koordinaten zu erhalten
* saubere Architektur durch mehrere Iterationen
  * regelmässig durchgeführte Reviews um die Code-Qualität hoch zu halten
  * durch die saubere Kapselung und Docker konnte das Deployment problemlos und in kurzer Zeit durchgeführt werden
* Transparenz während der ganzen Arbeit
  * durch JIRA, Github und wöchentlichen Sitzung ist sichtbar, wo man steht und was bisher erreicht wurde
  * aktueller Stand der Doku immer ausgeliefert
  * Sitzungsprotokolle und Beschlüsse nachgeführt

## Wie wurde vorgegangen?

* Einarbeitung Problem-Domain
* lange Evaluation des Stand der Technik
* QGIS Tests für Visibility-Graph und SpiderWeb-Graph
* Evaluation der Fremdsysteme (Search.ch, Overpass, Routing-Engines)
* Umsetzung der Vorverarbeitung
* Umsetzung des multimodalen Routing
* Umsetzung des QGIS-Plugin
* zu jeder Zeit wurde die Doku nachgeführt


## Mit welchen Herausforderungen hatten wir zu kämpfen?

* extrem viel gemacht, aber wenig kam bei den Stakeholder rüber
  * Befürchtung: dass bei Bewertung nicht alles sichtbar ist
* Vorgehen wurde nicht klar kommuniziert
  * theoretischer Fokus der Arbeit verunmöglicht ein Release-Early und Release-Often (siehe Vorgehen)
  * darum finden wir das modernes SW-Engineering durchgeführt wurde
* unterschiedliche Erwartungshaltungen an den Prototyp (QGIS-Plugin)
  * Missverständis bei der Fokuslegung
  * für Proof of Concept und nicht für den produktiven Einsatz, darum wurden auch nicht gross Usability-Test angedacht
* Scope zu gross angesetzt
  * verlängerte Extrameile musste gegangen werden, um alle Anforderungen erfüllen zu können
  * hat mit der Aufgabenstellung, wie auch der unbekannten Problem-Domain zu tun
* In Sitzung beschlossene Beschlüsse werden rückgängig gemacht

## Ein Lob an den Betreuer

* hat uns ausgiebig seine Zeit, Know-How und Kontakte zur Verfügung gestellt
* gestaltet aktiv mit, führt Recherche durch, interessiert sich für die Thematik
* steht voll hinter dem Projekt und gestaltet motiviert mit
* jederzeit erreichbar

## Was erhoffen wir uns zusätzlich für die BA

* häufiger und bewusster Ergebnisse demonstieren
* konrekter Feedback-Zyklus schon zu Beginn des Projekts
* Festlegung der konkreten Stakeholder und welchen Einfluss sie nehmen können und dürfen
* Abnahme der konkreten Projektplanung
* Festlegung, wann Anforderungen verändert oder eingeführt werden können
 * Beispielsweise während dem Weekly-Meeting, so dass sie in Sprint Planning aufgenommen werden können
 * im gleichen Schritt definieren, was sie für Auswirkungen auf den Scope haben
