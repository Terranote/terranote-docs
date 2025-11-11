# Operación y Runbooks

## Despliegues

- **Desarrollo**: utilizar `terranote-infra` con perfiles `core,fakes,observability`. Instrucciones detalladas en su [README](https://github.com/Terranote/terranote-infra/blob/main/README.md).
- **Staging/Producción**: definir pipelines de CI/CD compartidos (próximos pasos). Documentar variables sensibles en un gestor seguro.

## Runbooks sugeridos

1. **Fallo en publicación OSM**
   - Revisar métricas `terranote_note_publication_*` en Prometheus.
   - Verificar logs del core (`docker compose logs terranote-core`).
   - Cambiar el fake OSM a modo `network_error` para reproducir.
2. **Alertas de latencia**
   - Consultar dashboards (Grafana si está habilitado).
   - Analizar colas de mensajes en adaptadores.
   - Ajustar `OSM_API_TIMEOUT_SECONDS`/`OSM_MAX_RETRIES` según necesidad.

## Métricas y observabilidad

- Métricas expuestas por el core: ver tabla en [`docs/overview.md`](https://github.com/Terranote/terranote-core/blob/main/docs/overview.md).
- Scrape Prometheus: configurado en `docker/compose.prometheus.yml` de `terranote-core`.
- Logs estructurados: definir exportación a Loki/ELK (pendiente).

## Responsables

- **SRE/Infra**: mantener dashboards, monitorización y runbooks.
- **Core**: asegurar instrumentación adecuada en el servicio.
- **Adaptadores**: monitorear la entrega de notificaciones y salud de webhooks.

