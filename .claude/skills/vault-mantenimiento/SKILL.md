---
name: vault-mantenimiento
description: Audita la salud de la bóveda de Obsidian frente a CLAUDE.md - enlaces rotos, notas huérfanas, notas sin "🔗 Relacionado", nombres de archivo que no son minúsculas-con-guiones, tags inconsistentes, estados desincronizados - y propone arreglos. Úsalo cuando el usuario pida limpiar, ordenar, revisar o auditar la bóveda.
---

# Mantenimiento de la bóveda

## Flujo: auditar → informar → arreglar con permiso
1. **Inventario** de `.md` (excluye `.obsidian/`, `templates/`, `.claude/`).
2. **Comprobaciones**:
   - Enlaces rotos: `[[X]]` sin nota `X.md` (ten en cuenta alias `|`, `#secciones` y plantillas vacías `[[]]`).
   - Huérfanas: nadie las enlaza y no enlazan a nada.
   - Falta la sección `## 🔗 Relacionado`.
   - Nombre de archivo que no es `minusculas-con-guiones.md` (las diarias: `YYYY-MM-DD.md`).
   - Nota en carpeta equivocada (p. ej. `#persona` fuera de `personas/`).
   - Proyecto con `estado:` distinto de su tag `#estado/...`.
   - Tags con variantes (`#Idea`, `#ideas`) o `#tema/categoria` sin sustituir.
   - `inbox/` con notas de más de 7 días.
   - Duplicados probables (títulos casi iguales).
3. **Informe**: tabla corta problema → nota → arreglo, ordenada por impacto.
4. **Arreglos** solo tras confirmación, en lotes pequeños. Registra cada uno en `.claude/registro.md`.

## Reglas
- Nunca elimines; propón y pregunta.
- Al renombrar o mover, actualiza todos los enlaces entrantes.
- No toques `.obsidian/` ni binarios (sprites, pdf, piskel).
