---
name: vault-captura
description: Captura rápida de ideas, tareas o apuntes en la bóveda de Obsidian (nota diaria de hoy o inbox/) sin interrumpir el flujo del usuario. Úsalo cuando el usuario diga "apunta", "anota", "guarda esta idea", "recuérdame", haga un braindump o dicte pensamientos sueltos.
---

# Captura rápida

Guarda en segundos; se clasifica después con `vault-inbox`.

## Destino
- **Pensamiento, tarea o idea del día** → nota de hoy `daily-notes/YYYY-MM-DD.md`. Si no existe, créala desde `templates/daily-note.md` (sustituye `{{date:YYYY-MM-DD}}`).
  - Pensamiento / braindump → `## 🧠 Ideas / pensamientos`
  - Idea concreta → `## 💡 Ideas que surgieron` como `- #idea texto`
  - Tarea → `## 🎯 Objetivos` como `- [ ] texto`
- **Material sin contexto** (enlace, texto pegado, dato suelto) → `inbox/YYYY-MM-DD-titulo-corto.md` con `#inbox` al final.

## Reglas
- No hagas preguntas.
- Conserva las palabras del usuario; no reescribas ni amplíes.
- Varias ideas en un mensaje → una viñeta por idea.
- Si menciona un proyecto, persona o nota existente, enlázalo con `[[...]]`.

## Respuesta
Una sola línea: `Guardado en [[destino]]`.
