# Estándares y Buenas Prácticas

## Estilo de código

- Python: seguir PEP8, formatear con `black`, lint con `ruff`.
- Testing: usar `pytest`, marcadores `smoke`, `e2e`, `load` para clasificar suites.

## Revisiones y PR

- Requerir al menos 1 aprobación del equipo correspondiente.
- Adjuntar enlaces a pruebas ejecutadas (`pytest`, `docker compose`, etc.).
- Actualizar documentación relevante (`terranote-docs` o repos locales) cuando cambien flujos.

## Seguridad

- Secretos gestionados a través de variables de entorno y herramientas secret manager (pendiente especificar).
- Nunca commitear `.env` ni claves API.

## Versionado

- Tags alineados por fases (ej. `v1.0.0-fase1` para core/adaptadores).
- `main` como rama estable; usar ramas `feature/`, `hotfix/` para cambios.

## Pruebas mínimas

- Core: `pytest --cov` y validación de interfaces.
- Infra: pruebas de `docker compose` en CI.
- Tests: ejecutar `pytest -m smoke` para gating de cambios.

