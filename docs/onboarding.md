# Onboarding de Terranote

## Prerrequisitos

- Python 3.11+ y Poetry 1.8+.
- Docker Engine o Desktop (4 GB RAM disponibles).
- Acceso a los repositorios de Terranote.

## Checklist inicial

1. Clonar los repositorios principales en el mismo directorio:
   ```bash
   git clone https://github.com/Terranote/terranote-core.git
   git clone https://github.com/Terranote/terranote-infra.git
   git clone https://github.com/Terranote/terranote-tests.git
   ```
2. Configurar entorno virtual y dependencias en `terranote-core` (ver [README](https://github.com/Terranote/terranote-core/blob/main/README.md)).
3. Preparar `terranote-infra` copiando `.env.example` a `.env` y ajustando variables necesarias ([README](https://github.com/Terranote/terranote-infra/blob/main/README.md)).
4. Instalar dependencias de pruebas en `terranote-tests`:
   ```bash
   cd terranote-tests
   poetry install
   ```
5. Revisar guías de adaptadores si trabajarás con un canal específico (ej. [WhatsApp](https://github.com/Terranote/terranote-adapter-whatsapp/blob/main/README.md)).

## Primeros pasos recomendados

- Ejecutar la [guía E2E](https://github.com/Terranote/terranote-core/blob/main/docs/e2e-guide.md) para validar el flujo end-to-end.
- Leer los [contratos de interacción](https://github.com/Terranote/terranote-core/blob/main/docs/interfaces.md) para entender la API.
- Explorar los escenarios de prueba disponibles en `terranote-tests` ([README](https://github.com/Terranote/terranote-tests/blob/main/README.md)).

## Contactos y soporte

- Canal principal (Product Owner y equipo técnico): Telegram `https://t.me/osm_notes_latam`. Actualmente la coordinación está a cargo de Angie; en el futuro se integrará Rafael (`risturiz`).
- TODO: definir y publicar el correo de contacto oficial cuando esté disponible.

