# Day 02 – Container Orchestration

## Grundidee
Container-Orchestrierung verwaltet Container über mehrere Hosts hinweg,
um Skalierbarkeit, Ausfallsicherheit und Automatisierung zu ermöglichen.

## Warum das wichtig ist
Container auf einem einzelnen Host zu betreiben skaliert nicht
und erzeugt Single Points of Failure.

Orchestratoren wie Kubernetes automatisieren:
- Neustarts
- Platzierung von Workloads
- Skalierung

## Kernaussage
**Container verpacken Anwendungen.  
Orchestratoren betreiben Systeme.**

---

## Container – kurze Wiederholung

- Container sind isolierte Prozesse, die sich den Kernel des Host-Systems teilen
- Sie bündeln Anwendungen inklusive Abhängigkeiten
- Container-Images sind unveränderliche Vorlagen
- Container sind laufende Instanzen dieser Images

---

## Was ist Container-Orchestrierung?

Der Betrieb von Containern auf einem einzelnen Host ist für Entwicklung oft ausreichend.
In QA- und Produktionsumgebungen stößt dieser Ansatz jedoch schnell an Grenzen.

Produktionssysteme erfordern:
- Ausfallsicherheit
- Bedarfsorientierte Skalierung
- Effiziente Ressourcennutzung
- Service Discovery
- Externe Erreichbarkeit
- Zero-Downtime-Updates und Rollbacks

Container-Orchestratoren fassen mehrere Hosts zu einem Cluster zusammen
und automatisieren den gesamten Lebenszyklus von Containern im großen Maßstab.

Dadurch entsteht ein verteiltes System mit höherer
Zuverlässigkeit, Performance und Kosteneffizienz.

---

## Überblick: Container-Orchestrierungswerkzeuge

Es existieren verschiedene Container-Orchestratoren,
häufig an bestimmte Cloud-Anbieter gebunden.

- **ECS / ACI**  
  Verwaltete, cloud-spezifische Lösungen

- **Docker Swarm**  
  Technisch ein Orchestrator, in der Praxis heute kaum noch relevant

- **Nomad**  
  Nischenlösung, oft im HashiCorp-Ökosystem eingesetzt

- **Kubernetes**  
  Open-Source-Standard, CNCF-Projekt, weit verbreitet im Produktiveinsatz

---

## Kernaussage
Kubernetes hat sich als Industriestandard für Container-Orchestrierung etabliert.
Die meisten Alternativen sind entweder herstellerspezifisch oder Nischenlösungen.

---

## Warum Container-Orchestratoren einsetzen?

Die manuelle Verwaltung weniger Container oder einfache Skripte funktionieren nur im kleinen Maßstab.
Bei Hunderten oder Tausenden Containern ist dieser Ansatz nicht mehr tragfähig.

Container-Orchestratoren lösen dieses Problem durch:

- Zusammenfassung mehrerer Hosts zu einem logischen Gesamtsystem
- Automatisches Scheduling anhand verfügbarer Ressourcen
- Service-zu-Service-Kommunikation über Host-Grenzen hinweg
- Verwaltung von Storage und Container-Lebenszyklen
- Load Balancing und stabile Zugriffspunkte
- Optimierte Ressourcennutzung
- Durchsetzung von Sicherheits- und Zugriffsrichtlinien

---

## Fazit
Container-Orchestratoren machen aus vielen einzelnen Maschinen
ein zuverlässiges, automatisiert betriebenes System.

Kubernetes ist die am weitesten verbreitete Lösung für dieses Problem.
