\# Woche 2: Hub-and-Spoke-Netzwerk



\## Ziel

Hub-and-Spoke-Topologie als Bicep-Code mit VNet-Peering.



\## Umsetzung

\- Modul `bicep/modules/vnet.bicep` für wiederverwendbare VNets

\- Hub `10.0.0.0/16` mit Subnetz `snet-shared`

\- Spoke `10.1.0.0/16` mit Subnetzen `snet-app` und `snet-data`

\- Peerings in beide Richtungen

\- Pipeline validiert mit `az bicep build` und `az bicep lint`



\## Offen

\- `what-if` und Deployment erst, wenn das Azure-Abo aktiv ist



\## Erkenntnisse

\- Peerings müssen in beide Richtungen angelegt werden

\- Modul-Outputs (`hub.outputs.id`) erzwingen die Reihenfolge der Ressourcen

