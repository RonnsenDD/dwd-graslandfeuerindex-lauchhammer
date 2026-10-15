# DWD-Graslandfeuerindex Lauchhammer

Öffentlicher Feed der DWD-Station **Schipkau-Klettwitz (Stationskennung 2627)**.

Quelle: [DWD Open Data – Graslandfeuerindex](https://opendata.dwd.de/climate_environment/CDC/derived_germany/fire_danger_index/grassland/forecast/recent/). Die Datei enthält heute und bis zu sechs Vorhersagetage. Der private Abrufworkflow aktualisiert täglich um 05:15 UTC und kann manuell gestartet werden.

Das JSON-Schema enthält `schemaVersion`, `station`, `status`, `retrievedAt`, `source`, `today` und `days`. Jeder Tageswert enthält ein ISO-Datum und einen Index der DWD-Klassen 1 bis 5. `status` ist `ok`, `stale` oder `error`; bei Fehlern werden ausschließlich zuvor validierte Werte als `stale` weitergegeben. Ein `error`-Dokument ohne gültige Werte wird nicht veröffentlicht.
