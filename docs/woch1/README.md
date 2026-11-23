\# Woche 1: Identität, Governance und Pipeline



\## Ziel

Managed Identity mit minimalen Rechten, Azure Policy für erlaubte Regionen und eine Validierungspipeline für Bicep.



\## Umsetzung

\- Bicep-Datei `bicep/main.bicep` (VNet als Startpunkt)

\- Pipeline `.github/workflows/validate.yml` validiert die Bicep-Datei bei jedem Push

\- Erster Lauf erfolgreich (grüner Haken im Tab Actions)



\## Offen

\- Managed Identity, RBAC und Policy noch nicht umgesetzt: Azure-Abo ist deaktiviert (schreibgeschützt)

\- Nachholen, sobald ein aktives Abo verfügbar ist



\## Erkenntnisse

\- YAML reagiert empfindlich auf Tabs und Einrückung

\- Beim Speichern in Notepad auf „Alle Dateien“ und UTF-8 achten, sonst entsteht eine `.txt`-Endung

