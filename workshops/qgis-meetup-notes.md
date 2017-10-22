# QGIS Meetup
- [Etherpad](https://etherpad.coredump.ch/p/QGIS_Devs_Meetup_HSR)
- QML als deskriptive Sprache für Qt
- DevDocs QGis Python API

## Plugin-Development
- Logging, `prints` sind gefährlich
    - in QGIS Message log
    - `qgis.QgsMessageLog.logMessage`
- `QgsNetworkAccessManager`
- `pyqtslot`: subscriber
- `QString` für String-Parameter

- Python multiprocessing, kann multi-core nutzen
    - z.B. `mp.Pool().umap_unordered()`

## Tooling
- pyCharm Debugging (nur mit Professional version)
- new Run configuration
    - python remote debug

### QGis Layer
- Braucht normalerweise Datenquelle
    - Wie, wenn Features manuell hinzugefügt werden? In Projekt gespeichert?

### Qt
- am besten Tabellen-Layouts verwenden
