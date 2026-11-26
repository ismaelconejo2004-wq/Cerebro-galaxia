---
name: vault-diario
description: Crea o abre la nota diaria de hoy en daily-notes/ desde templates/daily-note.md, arrastrando los objetivos pendientes del último día. Úsalo cuando el usuario diga "nota de hoy", "empieza el día", "/diario", "planifica hoy" o pida cerrar el día con una reflexión.
---

# Nota diaria

Ruta: `daily-notes/YYYY-MM-DD.md` (fecha local de hoy). Plantilla: `templates/daily-note.md`.

## Empezar el día
1. Si la nota de hoy existe, léela y no la recrees.
2. Busca la nota anterior más reciente en `daily-notes/` (no siempre es ayer).
3. Copia sus objetivos sin completar (`- [ ]`) a `## 🎯 Objetivos` de hoy con su origen: `- [ ] tarea ([[2026-11-25]])`. En la nota anterior márcalos `- [>]` (movido); no los borres.
4. Crea la nota desde la plantilla sustituyendo `{{date:YYYY-MM-DD}}`.
5. En `## 🔗 Referencias` enlaza la nota anterior y los proyectos con `estado: activo` de `proyectos/`.

## Cerrar el día (si lo pide)
- Mueve a `## ✅ Completado` lo que el usuario diga que hizo, como `- [x]`.
- Las ideas que salieron van a `## 💡 Ideas que surgieron` con `#idea`.
- Usa sus palabras; pregunta si no lo ha dicho.

## Respuesta
Una línea con el enlace a la nota y cuántos objetivos se arrastraron.
