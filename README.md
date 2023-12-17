# DevOps Projectopdracht - Zakaria El Habib

## Beschrijving
Dit project omvat een geïntegreerde omgeving met een front-end in Nginx, een back-end in Node.js en een MySQL-database, allemaal gehost in afzonderlijke Docker-containers. Deze services worden beheerd en gecoördineerd via Docker Compose. Traefik wordt gebruikt als reverse proxy, als tussenliggende server om inkomende clientverzoeken te ontvangen en door te sturen naar de juiste servers. Daarnaast is er een geautomatiseerde CI/CD-pijplijn geïmplementeerd met Jenkins voor continue integratie en deployment.

## Installatie-instructies + gebruik
1. Clone deze repository met het commando `git clone <repository_url>`.
2. Download Docker en Docker Compose op je lokale machine.
3. Stel de 'docker-compose.yml'-bestanden in de 'jenkins' en 'traefik'-mappen zo in dat je de gewenste URL kunt gebruiken om naar het Jenkins- of Traefik-dashboard te navigeren.
4. Start Jenkins en Traefik door naar de map 'traefik' of 'jenkins' te gaan en het commando `docker-compose up` (of `docker-compose up -d` voor de achtergrondmodus) uit te voeren.
5. Configureer het `docker-compose.yml`-bestand voor zowel de front-end als de back-end, zodat je de gewenste URL voor de website kunt instellen (zorg ervoor dat dit hetzelfde is).
6. Start de front-end, back-end en MySQL-containers met het commando `docker-compose up` of `docker-compose up -d`.
7. Zorg ervoor dat je een geldig TLS-certificaat hebt.
8. Ga naar de URL die je hebt ingesteld in het `docker-compose.yml`-bestand om de website te bekijken.
9. Ga naar de URL die je hebt ingesteld in de 'traefik'-map om naar het Traefik-dashboard te gaan. Hier heb je een overzicht van de routeringsregels, backend-services, verkeersstatistieken en gezondheidsstatussen van de gehoste services (je front en backend).
10. Ga naar de URL die je hebt ingesteld in de 'jenkins'-map om naar het Jenkins-dashboard te gaan.
    
