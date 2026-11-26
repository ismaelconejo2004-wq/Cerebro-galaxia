---
name: vault-buscar
description: Busca y sintetiza información dentro de la bóveda de Obsidian (proyectos, personas, research, ideas, notas diarias) citando las notas de origen. Úsalo cuando el usuario pregunte "qué tengo sobre...", "qué hablé con...", "busca en mis notas", "encuentra", o haga falta contexto de la bóveda antes de responder.
---

# Buscar en la bóveda

## Procedimiento
1. Saca 2-4 palabras clave y sinónimos.
2. Acota por carpeta según la pregunta: persona → `personas/`, herramienta/artículo → `research/`, "qué hice" → `daily-notes/`, proyecto → `proyectos/`.
3. Busca por nombre de archivo (Glob), luego por contenido (Grep `-i`, `glob: "*.md"`), y por tags (`#tema/...`, `#estado/...`, `#prioridad/...`) o frontmatter (`estado:`, `relevancia:`).
4. Lee solo las notas relevantes y sigue un nivel de `[[enlaces]]` desde `🔗 Relacionado`.

## Respuesta
- Sintetiza; no vuelques notas completas.
- Cita cada dato con `[[nota]]`.
- Separa lo que dicen las notas de tu inferencia.
- Sin resultados: dilo y sugiere otros términos; no inventes.
- Ignora `.obsidian/`, `templates/` y binarios.

Solo lectura. Para guardar el resultado, usa `vault-nota`.
