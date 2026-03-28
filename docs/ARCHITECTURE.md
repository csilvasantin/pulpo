# Arquitectura de Pulpo

## Vision tecnica

Pulpo es un orquestador de IAs que recibe una tarea grande, la descompone en subtareas y las asigna a IAs especializadas. Cada IA trabaja en su rama de Git y Pulpo unifica los resultados.

## Componentes principales

```
                    +------------------+
                    |    CEO (Carlos)  |
                    |   Asigna tareas  |
                    +--------+---------+
                             |
                    +--------v---------+
                    |   TASKS.md       |
                    |   Tablero central|
                    +--------+---------+
                             |
              +--------------+--------------+
              |                             |
    +---------v----------+       +----------v---------+
    |   CTO (Claude)     |       |   CMO (Codex)      |
    |   rama: claude/*   |       |   rama: codex/*    |
    |   Tecnologia       |       |   Marketing        |
    +--------------------+       +--------------------+
```

## Modulos del producto (futuro)

```
src/
  index.ts              CLI entry point
  core/
    task-decomposer.ts  Descompone tareas grandes en subtareas
    task-runner.ts       Ejecuta y coordina subtareas
    result-aggregator.ts Une resultados de todas las IAs
  ai/
    registry.ts         Registro de IAs disponibles
    claude-adapter.ts   Adapter para Claude CLI
    codex-adapter.ts    Adapter para Codex CLI
  coordination/
    git-coordinator.ts  Gestion de ramas y PRs
    state-manager.ts    Estado en JSON
    task-file.ts        Generacion de TASKS.md
  types/
    index.ts            Interfaces TypeScript
  utils/
    shell.ts            Ejecucion de procesos
    logger.ts           Logging
    git.ts              Helpers git
```

## Stack

- **Runtime**: Node.js
- **Lenguaje**: TypeScript
- **CLI**: Commander
- **Estado**: JSON files en `.pulpo/`
- **Coordinacion**: GitHub (ramas + TASKS.md)
- **Dependencias**: minimas — uuid, chalk, commander

## Principios

1. Simplicidad primero — no sobreingenieria
2. Cada IA trabaja en aislamiento (su propia rama)
3. TASKS.md como fuente de verdad
4. El CEO es el unico que mergea a main
5. Extensible — nuevas IAs = nuevo archivo de rol + prefijo de rama
