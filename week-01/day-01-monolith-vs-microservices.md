# Day 01 – Monolith vs. Microservices

## Was ich heute gelernt habe
- Unterschied zwischen monolithischen Anwendungen und Microservices
- Warum Monolithen im Cloud-Betrieb schwer skalierbar und wartbar sind
- Zentrale Vorteile von Microservices: Entkopplung, Modularität, unabhängige Skalierung
- Warum Container ein entscheidender Enabler für Microservices sind

## Tools / Plattformen
- Linux Foundation – Introduction to Kubernetes (LFS158)

---

## Monolith

- Eine große, zusammenhängende Anwendung  
- Komponenten sind stark miteinander gekoppelt  
- Skalierung nur als Gesamtsystem möglich  
- Updates verursachen meist Downtime  
- Hoher Hardwarebedarf  
- Wartung und Weiterentwicklung werden mit der Zeit schwierig  

**Merksatz:**  
**Monolith = ein großer Block, schwer zu bewegen**

---

## Microservices

- Viele kleine, lose gekoppelte Services  
- Jeder Service hat eine klar definierte Aufgabe  
- Kommunikation über APIs  
- Jeder Service kann unabhängig skaliert werden  
- Updates ohne Downtime möglich  

**Merksatz:**  
**Microservices = viele kleine Bausteine**

---

## Refactoring – Realität

- „Big-Bang“-Refactoring → hohes Risiko  
- Inkrementelles Refactoring → realistischer Ansatz  
- Legacy-Monolithen (COBOL, Mainframe, stark gekoppelte Datenbanken)  
  → oft sinnvoller neu zu bauen als zu refactoren  

---

## Eigene Reflexion
- Viele dieser Probleme habe ich selbst beim Betrieb von Nextcloud AIO erlebt
- Das hat mir geholfen zu verstehen, warum Kubernetes und Container reale operative Probleme lösen
