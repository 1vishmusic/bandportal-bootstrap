# bandportal - Semestrální práce k předmětu BI-TJV

Jedná se o systém databáze koncertů kapely, ve kterém bude jednoduše možné vytvářet a upravovat koncerty. Hlavním výstupem z tohoto systému by měla být api, ze které se snadno vygeneruje seznam koncertů pro oficiální stránky kapely.

## Databázový diagram

![image](/assets/diagram.png)

## Dotaz

Zjištění všech neproběhlých koncertů

## Business operace

Vytvoření události v době, kdy se nekoná jiná událost.

## Spuštění

1) Ke spuštění je potřeba docker a docker-compose (případně podman a podman-compose, ale postup s podmanem jsem nezkoušel)
2) Je třeba se přihlásit do FIT sítě přes VPN, pokud nejsme na školním PC. Některé příkazy použité níže mohou potřebovat ```sudo```.
3) ```docker login gitlab.fit.cvut.cz:5050``` nebo ```podman login gitlab.fit.cvut.cz:5050```
4) ```docker-compose up``` nebo ```podman-compose up```
5) Dashboard (správce) by měl být dostupný na adrese [http://localhost:3000](http://localhost:3000), Rest API ne adrese [http://localhost:8080](http://localhost:8080)