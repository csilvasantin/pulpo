# Reglas de Colaboracion — Pulpo

Estas reglas aplican a TODAS las IAs del equipo. Leelas antes de hacer cualquier cosa.

## 1. Antes de actuar

- Lee `RULES.md` (este archivo)
- Lee `TASKS.md` para ver que te toca
- Lee `STATE.md` para saber donde estamos
- Lee tu archivo de rol (`CLAUDE.md` o `CODEX.md`) para tu contexto especifico

## 2. Ramas

- Cada IA trabaja en su propia rama
- Claude: `claude/<nombre-tarea>`
- Codex: `codex/<nombre-tarea>`
- **Nunca pushear a main directamente** — solo via PR o merge aprobado por el CEO

## 3. Tareas

- Solo trabaja en tareas asignadas a ti en `TASKS.md`
- No toques tareas de otra IA
- Al terminar, actualiza tu tarea en `TASKS.md` con estado `completada`
- Si te bloqueas, cambia estado a `bloqueada` y explica en la columna Notas

## 4. Commits

- Mensajes claros en espanol
- Prefijo con tu rol: `[CTO]`, `[CMO]`
- Ejemplo: `[CTO] Implementar tipos base de PulpoTask`

## 5. Codigo

- Mantener cambios pequenos y enfocados
- No borrar trabajo de otra IA sin aprobacion del CEO
- Documentar decisiones importantes en `docs/`
- Preferir claridad sobre cleverness

## 6. Conflictos

- Si dos IAs necesitan el mismo archivo, el CEO decide prioridad
- Nunca resolver conflictos de merge sobreescribiendo trabajo ajeno

## 7. Comunicacion

- Toda comunicacion pasa por los archivos del repo
- `TASKS.md` es la fuente de verdad para asignaciones
- `STATE.md` es la fuente de verdad para el estado del proyecto
- Si necesitas algo de otra IA, anadelo como nota en `TASKS.md`

## 8. Nuevos miembros

- Cuando se una una nueva IA, se crea `<NOMBRE>.md` con su rol y contexto
- Se anade a la tabla del equipo en `README.md`
- Se le asigna un prefijo de rama propio
