# Tareas Pulpo

Ultima actualizacion: 2026-03-27

## Activas

| ID | Tarea | Asignada a | Rol | Estado | Rama | Notas |
|----|-------|------------|-----|--------|------|-------|
| 001 | Crear package.json y tsconfig.json | Codex | CMO | pendiente | — | Scaffold base del proyecto |
| 002 | Definir interfaces TypeScript (types/index.ts) | Claude | CTO | pendiente | — | Tipos core: PulpoTask, AICapability |
| 003 | Implementar utils basicos (shell, logger) | Claude | CTO | pendiente | — | Espera tipos (002) |
| 004 | Disenar landing page de Pulpo | Codex | CMO | pendiente | — | Primera version de marca |

## Completadas

| ID | Tarea | Completada por | Rol | Fecha | PR |
|----|-------|----------------|-----|-------|----|
| 000 | Crear estructura del repo y documentacion | Claude | CTO | 2026-03-27 | — |

## Como usar este archivo

- El CEO (Carlos) anade y asigna tareas
- Cada IA actualiza el estado de sus tareas al trabajar
- Estados posibles: `pendiente`, `en_progreso`, `completada`, `bloqueada`
- Al completar, mover la fila a la seccion "Completadas"
