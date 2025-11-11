# Anexos

## Plantillas sugeridas

- Plantilla de Pull Request (pendiente de crear en `.github/pull_request_template.md`).
- Formato de reporte de incidente (guardar en `docs/templates/incident-report.md` cuando esté disponible).

## Decisiones de arquitectura (ADR)

- Registrar futuras decisiones en `docs/adr/ADR-XXXX.md`.
- Incluir contexto, decisión, alternativas consideradas e impacto.

## Preguntas frecuentes

- **¿Cómo ejecuto pruebas rápidas?**  
  Usa `poetry run pytest -m smoke` desde `terranote-tests` tras levantar la infraestructura.
- **¿Puedo usar la API de OSM real en desarrollo?**  
  Se recomienda utilizar el fake incluido para evitar saturar la API oficial.
- **¿Dónde reporto bugs?**  
  Abrir issue en el repositorio correspondiente y etiquetar al Product Owner.

## Historial

- `2025-11-11`: Creación inicial de la estructura documental.
- Próximos hitos: incorporar diagramas adicionales y runbooks específicos por incidente.

