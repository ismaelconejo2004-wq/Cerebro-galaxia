---
name: vault-inbox
description: Procesa la carpeta inbox/ y las ideas sueltas de las notas diarias de la bóveda de Obsidian y las convierte en notas de proyecto, persona, research o idea con su plantilla, previa confirmación. Úsalo cuando el usuario pida "procesar el inbox", "clasificar", "ordenar lo apuntado" o "vaciar la bandeja".
---

# Procesar el inbox

## Fuentes
- Todos los `.md` de `inbox/` y las notas con `#inbox`.
- Viñetas `#idea` de `## 💡 Ideas que surgieron` en `daily-notes/` aún sin procesar (las procesadas llevan ` ✅ → [[destino]]`).

## Procedimiento
1. Reúne los elementos pendientes.
2. Propón un destino para cada uno:
   - Tarea de un proyecto → `## ✅ Próximos pasos` del proyecto.
   - Persona → `personas/` (`templates/persona.md`).
   - Artículo, herramienta → `research/` (`templates/research.md`).
   - Idea → `ideas/`; si ya está madura, proyecto nuevo con `templates/proyecto.md`.
   - Referencia estática → `resources/`.
   - Amplía una nota existente → añadirlo ahí.
3. Muestra la propuesta en una tabla (elemento → destino) y **espera confirmación**.
4. Aplica con `vault-nota`. En las notas diarias marca el origen ` ✅ → [[destino]]`. Las notas de `inbox/` ya convertidas se mueven al destino (no se borran); quita `#inbox`.
5. Registra cada acción al final de `.claude/registro.md`: `YYYY-MM-DD HH:MM · inbox · origen → destino`.

## Respuesta
N procesados, M notas nuevas, K tareas añadidas, lo que quedó pendiente.
