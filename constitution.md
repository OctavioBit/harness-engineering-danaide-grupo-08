# Constitución · Mesa de Ayuda
## Misión
API de tickets de soporte con SLA por prioridad y escalamiento en tres niveles.
Para: soporte y producto (Martín), operaciones (Sofía). La mantiene ingeniería (Lucía).
## Stack
Python 3.12 + FastAPI · PostgreSQL (SQLite en tests) · pytest · Docker Compose.
## Calidad
- Primero el test. Cada criterio R<n> del spec tiene al menos un test.
- Todo cambio entra por merge request con revisión humana.
## Seguridad y datos
- Solo datos sintéticos.
- Ningún secreto en el repo: configuración por variables de entorno.
## Forma de trabajo
- El orden de trabajo vive en specs/backlog.md: fases chicas, una por historia MDA-n.
- Un spec por fase en specs/NNN-<slug>/, enlazado a su historia.
- Si el comportamiento cambia, cambia primero el spec.