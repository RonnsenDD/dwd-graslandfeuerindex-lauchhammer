# DWD-Graslandfeuerindex Lauchhammer

Öffentlicher DWD-Feed der Station **Schipkau-Klettwitz (Stationskennung 2627)**.

Die Daten stammen aus der offiziellen [DWD Open-Data-Prognose](https://opendata.dwd.de/climate_environment/CDC/derived_germany/fire_danger_index/grassland/forecast/recent/). Der private Abrufworkflow aktualisiert die Datei täglich um 05:15 UTC und kann manuell gestartet werden. Die Quelldatei enthält den heutigen Index und bis zu sechs Vorhersagetage.

Das JSON enthält `schemaVersion`, `station`, `status`, `retrievedAt`, `source`, `today` und `days`. Tageswerte haben ein ISO-Datum und eine DWD-Indexklasse von 1 bis 5. Der Status lautet `ok`, `stale` oder `error`. Bei Fehlern werden nur zuvor geprüfte Werte als veraltet weitergegeben; ein Fehlerdokument ohne gültige Werte wird nicht veröffentlicht.
