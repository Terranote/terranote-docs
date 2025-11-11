# Introducción a Terranote

## Misión

Centralizar reportes ciudadanos de incidentes viales y urbanos y publicarlos como notas en OpenStreetMap para acelerar su resolución.

## Alcance

- Núcleo (`terranote-core`) que orquesta la recepción de interacciones, construcción de notas y publicación en OSM.
- Adaptadores oficiales (WhatsApp, Telegram, etc.) que capturan mensajes de los canales.
- Infraestructura compartida para ejecutar pruebas end-to-end, observabilidad y entornos de despliegue.

## Glosario

- **Interacción**: mensaje entrante de un usuario final gestionado por un adaptador.
- **Nota OSM**: entrada pública generada en OpenStreetMap que describe un incidente.
- **Fake OSM**: servicio emulado usado en pruebas para evitar depender de la API oficial.

## Enlaces rápidos

- Repositorios principales:
  - Núcleo: <https://github.com/Terranote/terranote-core>
  - Infraestructura: <https://github.com/Terranote/terranote-infra>
  - Pruebas: <https://github.com/Terranote/terranote-tests>
  - Adaptadores oficiales: <https://github.com/orgs/Terranote/repositories>
- Estrategia documental: [`docs/structure.md`](./structure.md)

