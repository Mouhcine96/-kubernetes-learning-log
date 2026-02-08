# Day 03 – Warum Container-Orchestratoren notwendig sind

## Problemstellung
Die manuelle Verwaltung einer kleinen Anzahl von Containern
– sei es per Hand oder über einfache Skripte –
funktioniert nur in sehr kleinen Umgebungen.

Sobald Systeme auf Hunderte oder Tausende Container anwachsen,
bricht dieser Ansatz unweigerlich zusammen.

Menschlich gesteuerter Betrieb skaliert nicht zuverlässig.

---

## Warum Orchestrierung erforderlich ist

Produktionsumgebungen stellen Anforderungen,
die durch manuelles Container-Management nicht erfüllt werden können:

- Ausfallsicherheit
- Bedarfsorientierte Skalierung
- Effiziente Ressourcennutzung
- Service Discovery
- Stabile externe Erreichbarkeit
- Zero-Downtime-Updates und Rollbacks

Diese Anforderungen gelten über mehrere Hosts,
Netzwerke und Umgebungen hinweg.

---

## Was Container-Orchestratoren leisten

Container-Orchestratoren lösen diese Probleme,
indem sie eine zentrale Steuerebene einführen,
die Container im großen Maßstab verwaltet.

Zentrale Fähigkeiten:

- **Clustering**  
  Mehrere Hosts werden zu einem logischen Gesamtsystem zusammengefasst.

- **Scheduling**  
  Container werden anhand verfügbarer Ressourcen auf Hosts verteilt.

- **Service-zu-Service-Kommunikation**  
  Container können hostübergreifend miteinander kommunizieren,
  ohne manuelle Netzwerkkonfiguration.

- **Storage-Anbindung**  
  Persistenter Speicher wird unabhängig vom Container-Lebenszyklus verwaltet.

- **Load Balancing & Abstraktion**  
  Mehrere Container-Instanzen werden als ein stabiler Service-Endpunkt bereitgestellt.

- **Ressourcenoptimierung**  
  CPU- und Speicherressourcen werden effizient im Cluster verteilt.

- **Sicherheit & Richtlinien**  
  Zugriffs- und Sicherheitsregeln werden zentral und konsistent durchgesetzt.

---

## Warum Kubernetes

Es existieren viele Orchestrierungswerkzeuge,
doch Kubernetes hat sich als Industriestandard etabliert.

Gründe dafür sind:
- Open Source
- Herstellerneutral
- CNCF-Unterstützung
- Großes Ökosystem
- Breite Nutzung im Produktivbetrieb

---

## Fazit
Container-Orchestratoren machen aus vielen einzelnen Maschinen
ein stabiles, automatisiert betriebenes Gesamtsystem.

Kubernetes ist die dominierende Lösung
für
