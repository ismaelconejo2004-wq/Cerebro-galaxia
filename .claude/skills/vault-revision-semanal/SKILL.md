---
name: vault-revision-semanal
description: Hace la revisión semanal de la bóveda de Obsidian - resume los últimos 7 días de daily-notes, el estado de los proyectos, tareas atascadas, personas sin seguimiento e inbox pendiente, y ayuda a planificar la semana. Úsalo cuando el usuario pida "revisión semanal", "resumen de la semana", "/semana" o planificar la próxima semana.
---

# Revisión semanal

Ruta: `daily-notes/YYYY-Www.md` (semana ISO, p. ej. `2026-W48`).

## Procedimiento
1. Lee las notas `daily-notes/YYYY-MM-DD.md` de los últimos 7 días.
2. Lee los proyectos de `proyectos/` con `estado: activo`.
3. Detecta:
   - Hecho: `## ✅ Completado` de cada día y decisiones nuevas en proyectos.
   - Atascado: objetivos arrastrados 3+ veces (`- [>]`).
   - Proyectos activos sin cambios en 14+ días (¿pasar a pausado?).
   - Personas con `ultima-interaccion` de hace 30+ días que aparecen en proyectos activos.
   - Pendiente en `inbox/` (sugiere `vault-inbox`).
4. Escribe la nota semanal:

```markdown
---
fecha: YYYY-MM-DD
tipo: semanal
---
# Semana YYYY-Www
Días: [[YYYY-MM-DD]] · ...

## ✅ Hecho
## ⚠️ Atascado
## 📁 Proyectos
| Proyecto | Estado | Siguiente paso |
## 👥 Seguimientos
## 💡 Aprendizajes
## 🎯 Foco próxima semana

## 🔗 Relacionado

---
#daily #semanal
```

5. Propón 3 prioridades para `🎯 Foco próxima semana` y deja que elija el usuario.

## Reglas
Cita cada afirmación con su nota. Solo escribe la nota semanal; para cambiar proyectos o estados, pregunta antes.
