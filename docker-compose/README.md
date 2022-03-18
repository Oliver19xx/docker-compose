# Übung: Docker-Compose

## Selber ausführen?

- Alles: `docker compose up -d` -> `docker composer down`
- Bestimmten Service und Abhängigkeiten: `docker compose up -d ui` (Startet api und ui) -> `docker compose down ui` (Stopt ui und api)

## Inhalt

- `Dockerfile`: Beschreibung des jeweiligen Containers
  - `.dockerignore`: Was soll der Container nicht sehen
- `docker-compose.yml`: Contaier orchestrieren
- `.env`: Umgebungsvariablen für docker compose
  - `(ui|api)/.env`: Umgebungsvariablen für die jeweiligen Container
- `profiles`: Markierung von Services um Gruppen von Services einzeln zu starten
- Netzwerke: Um Container expliziet untereinander zu verbinden

Quelle: [the native web GmbH - Docker-Compose: Eine Einführung in 80 Minuten // deutsch](https://www.youtube.com/watch?v=0jC5B9iTF_g&list=PLB8EM3vqHG59_xLE8Zz4M4vQVy-4RPCxR&index=5&ab_channel=thenativewebGmbH)