# Proposed Structure for Terranote Documentation

## Purpose

> Source of truth for documentation shared across the Terranote ecosystem. Defines dónde vive el contenido global y cómo enlaza a guías específicas en cada repositorio (incluyendo `terranote-core`, adaptadores y herramientas de prueba).

## Tabla de contenidos objetivo

1. **Introducción**
   - Misión y alcance de Terranote.
   - Glosario compartido.
   - Enlaces rápidos a repositorios principales.
2. **Arquitectura de plataforma**
   - Diagrama general del ecosistema.
   - Descripción de módulos (`core`, adaptadores, infraestructura, observabilidad).
   - Enlace a `terranote-core/docs/overview.md` para detalles internos del núcleo.
3. **Onboarding**
   - Requisitos de entorno y herramientas globales.
   - Checklist de primeros pasos (clonado de repos, cuentas externas).
   - Enlaces a guías locales:
     - `terranote-core/docs/e2e-guide.md`
     - `terranote-infra/README.md`
     - `terranote-tests/README.md`
4. **Operación y runbooks**
   - Procedimientos de despliegue (dev, staging, prod).
   - Runbooks para incidentes comunes.
   - Matriz de responsables (SRE, adaptadores, core).
5. **Estándares y buenas prácticas**
   - Guías de estilo, revisión y testing compartidas.
   - Políticas de seguridad y secretos.
   - Convenciones de ramas y versionado.
6. **Referencias por componente**
   - Resumen por repositorio con enlaces:
     - `terranote-core` → `README.md`, `docs/interfaces.md`, `docs/e2e-guide.md`.
     - `terranote-infra` → perfiles `docker-compose`, configuración `.env`.
     - `terranote-tests` → marcadores pytest, escenarios de carga.
     - Adaptadores oficiales (WhatsApp, Telegram, etc.).
7. **Anexos**
   - Plantillas (PR, incident report).
   - ADRs globales.
   - Preguntas frecuentes.

## Ownership y mantenimiento

- **Product Owner**: valida vigencia y prioriza cambios.
- **Equipo Core**: mantiene enlaces y resúmenes del núcleo.
- **Equipo Infra/SRE**: actualiza runbooks y despliegues.
- **Equipo QA/Tests**: mantiene referencias a `terranote-tests`.

Se recomienda una revisión trimestral coordinada por el Product Owner con checklist por equipo.

## Convenciones de enlaces cruzados

- En `terranote-docs`, enlazar a guías locales con rutas absolutas de GitHub (p. ej. `https://github.com/Terranote/terranote-core/blob/main/docs/e2e-guide.md`).
- En repos locales, incluir notas del tipo “Para contexto global, ver ...” apuntando a la sección correspondiente en este índice.
- Evitar duplicidad: contenido aplicable a múltiples repos debe residir aquí; los repos locales ofrecen resúmenes y enlaces.

