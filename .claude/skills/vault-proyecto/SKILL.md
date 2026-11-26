---
name: vault-proyecto
description: Crea o actualiza la nota de un proyecto en proyectos/ con templates/proyecto.md - estado, objetivos, decisiones clave, próximos pasos y relacionados. Úsalo cuando el usuario empiece un proyecto, convierta una idea en proyecto, registre una decisión, cambie el estado o pida el resumen o las tareas de un proyecto.
---

# Proyectos

Un archivo por proyecto: `proyectos/nombre-del-proyecto.md` (minúsculas, guiones). Plantilla: `templates/proyecto.md`.

## Crear
1. Comprueba que no exista ya (también en `ideas/`: si viene de una idea, enlaza la idea y añade a la idea `Convertida en [[proyecto]]`).
2. Crea desde la plantilla: `{{title}}` → nombre legible, `{{date:YYYY-MM-DD}}` → hoy.
3. Rellena descripción y objetivos con lo que dio el usuario; pregunta la fecha objetivo si no la dijo.

## Actualizar
- **Decisión** → nueva fila en `## 📌 Decisiones clave` con fecha y motivo. Nunca edites decisiones antiguas; añade una nueva que la sustituya.
- **Cambio de estado** → actualiza a la vez `estado:` del frontmatter y el tag final (`#estado/activo` | `#estado/pausado` | `#estado/completado`).
- **Tareas** → `## ✅ Próximos pasos`; marca `- [x]`, no borres las completadas.
- **Nota relacionada** → enlázala en `## 🔗 Relacionado` (Notas / Personas / Research).

## Resumen de estado
Lee el proyecto y las notas que lo enlazan (backlinks vía Grep `[[nombre]]`). Da: estado, últimas decisiones, próximos pasos y bloqueos.

## Recursos
Las imágenes, pdf y sprites no se mueven sin pedirlo. `proyectos/Proyecto DQ/` es una carpeta de recursos antigua: su nota de proyecto iría en `proyectos/proyecto-dq.md`, enlazando a esos recursos.
