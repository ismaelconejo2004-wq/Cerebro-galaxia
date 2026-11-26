---
name: vault-nota
description: Crea o edita notas en la bóveda de Obsidian usando la plantilla correcta de templates/ (proyecto, persona, research, idea) y las convenciones de CLAUDE.md. Úsalo cuando el usuario pida crear, redactar, desarrollar o reorganizar una nota, ficha de persona, investigación o documento. Para apuntes rápidos usa vault-captura.
---

# Crear y editar notas

Sintaxis de Obsidian: skill `obsidian:obsidian-markdown`. Convenciones: `CLAUDE.md`.

## Elegir tipo
| Si es... | Plantilla | Carpeta |
|---|---|---|
| Proyecto | `templates/proyecto.md` | `proyectos/` (o usa `vault-proyecto`) |
| Persona / contacto | `templates/persona.md` | `personas/` |
| Artículo, herramienta, investigación | `templates/research.md` | `research/` |
| Idea sin proyecto | estructura libre + `#idea` | `ideas/` |
| Material estático, cheatsheet | libre | `resources/` |
| Sin contexto suficiente | libre + `#inbox` | `inbox/` |

## Procedimiento
1. Busca si ya existe (Glob/Grep). Si existe, edítala; no dupliques.
2. Lee la plantilla y sustituye `{{title}}` por el título legible y `{{date:YYYY-MM-DD}}` por la fecha de hoy.
3. Nombre de archivo: minúsculas con guiones, sin tildes ni ñ (`juan-perez.md`, `herramientas-ia.md`). El H1 lleva el título legible.
4. Rellena solo con lo que dio el usuario; deja vacías las secciones sin datos.
5. Completa `🔗 Relacionado` con `[[enlaces]]` a notas que existan.
6. Conexiones inversas (CLAUDE.md):
   - Pertenece a un proyecto → añádela al `🔗 Relacionado` del proyecto.
   - Menciona una persona relevante → enlaza su nota en `personas/` o créala.
7. Research: cambia `#tema/categoria` por la categoría real (`#tema/ia`). Reutiliza tags existentes.

## Seguridad
Lee antes de sobrescribir. No borres. Al renombrar, actualiza los enlaces entrantes.

## Al terminar
Una línea: nota creada/editada y con qué notas quedó conectada.
