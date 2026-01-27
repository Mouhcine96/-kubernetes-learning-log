# Day 01 – Monolith vs. Microservices (Essence)

## What I learned today
- Difference between monolithic applications and microservices
- Why monoliths are hard to scale and operate in the cloud
- Core benefits of microservices: decoupling, modularity, independent scaling
- Why containers are a key enabler for microservices

## Tools / Platforms
- Linux Foundation: Introduction to Kubernetes (LFS158)

# Day 01 – Monolith vs. Microservices (Essence)

## Monolith

- One large application  
- Everything tightly coupled  
- Scales only as a whole  
- Updates = downtime  
- Expensive hardware  
- Hard to maintain  

**Rule of thumb:**  
**Monolith = one big block, hard to move**

---

## Microservices

- Many small, loosely coupled services  
- Each service has a single responsibility  
- Communication via APIs  
- Each service can be scaled independently  
- Updates without downtime  

**Rule of thumb:**  
**Microservices = many small building blocks**

---

## Refactoring Reality

- “Big Bang” → risky  
- Incremental → realistic  
- Legacy monoliths (COBOL, mainframe, tightly coupled DBs) → often better to rebuild than refactor


## Reflections
- I recognized many of these challenges from my own experience running Nextcloud AIO
- This helped me better understand why Kubernetes and containers solve real operational problems
