# Pulpo

Startup construida por humanos e IAs trabajando como un equipo real.

## El Equipo

| Rol | Nombre | Responsabilidad |
|-----|--------|-----------------|
| CEO | Carlos | Vision, decisiones estrategicas, direccion general |
| CTO | Claude | Arquitectura, codigo, decisiones tecnicas, infraestructura |
| CMO | Codex | Marketing, marca, landing pages, contenido, growth |

## Que es Pulpo

Una plataforma que orquesta multiples IAs para resolver tareas complejas. Un usuario da una tarea grande y Pulpo la reparte entre IAs especializadas, coordina el trabajo y unifica los resultados.

## Como funciona la colaboracion

1. El CEO asigna tareas en `TASKS.md`
2. Cada miembro del equipo lee `RULES.md` y `TASKS.md`
3. Trabaja en su rama (`claude/*`, `codex/*`)
4. Actualiza `TASKS.md` con el resultado
5. El CEO revisa y hace merge a main

## Archivos clave

| Archivo | Para que sirve |
|---------|---------------|
| `RULES.md` | Reglas de colaboracion para todo el equipo |
| `TASKS.md` | Tablero de tareas: quien hace que |
| `STATE.md` | Estado actual del proyecto |
| `CLAUDE.md` | Contexto y rol del CTO (Claude) |
| `CODEX.md` | Contexto y rol del CMO (Codex) |
| `docs/ARCHITECTURE.md` | Arquitectura tecnica de Pulpo |

## Stack

- Node.js / TypeScript
- Minimal dependencies
- GitHub como centro de coordinacion

## Vision

Cada IA tiene un rol, lo perfecciona con el tiempo, y entre todos formamos un verdadero Dream Team. Nuevas IAs se incorporaran con nuevos roles segun crezca el equipo.
