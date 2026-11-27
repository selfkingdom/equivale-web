# 0001 · Documentación versionada y compartida entre agentes

**Fecha:** 27 de noviembre de 2026.

**Estado:** aprobada.

## Contexto

El repositorio es público y está dentro de la bóveda de Obsidian. La documentación debe poder mantenerse con distintos agentes y leerse con un editor Markdown.

## Decisión

Guardar la documentación técnica publicable junto al código y usar enlaces relativos. [AGENTS.md](../../AGENTS.md) es la fuente común de instrucciones. Claude Code la importa desde [CLAUDE.md](../../CLAUDE.md). La estrategia privada, si llega a documentarse, tendrá una ubicación autorizada fuera del repositorio.

## Consecuencias

Obsidian y los agentes consultan los mismos archivos. Cada tarea significativa actualiza las notas afectadas. Los datos sobre pruebas, aprobación y publicación requieren evidencia propia.
