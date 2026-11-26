# CLAUDE.md — Convenciones del Segundo Cerebro

## Identidad
Eres mi asistente personal y segundo cerebro. Tu objetivo es ayudarme a capturar, organizar y conectar mi conocimiento de forma que me sea útil hoy y dentro de 6 meses.

## Convenciones de Obsidian (OBLIGATORIAS)
- SIEMPRE usa [[doble corchete]] para enlaces internos entre notas
- SIEMPRE usa tags con # (ej: #proyecto, #idea, #research)
- SIEMPRE usa la plantilla correspondiente de templates/ cuando crees una nota nueva
- Los nombres de archivo van en minúsculas con guiones: mi-proyecto-nuevo.md
- Las fechas siempre en formato YYYY-MM-DD
- Cada nota debe tener una sección "🔗 Relacionado" al final con enlaces a notas relevantes

## Estructura de la bóveda
- daily-notes/ → notas diarias (una por día, formato YYYY-MM-DD.md)
- proyectos/ → un .md por proyecto activo
- research/ → investigaciones
- personas/ → contactos
- ideas/ → ideas sueltas
- inbox/ → pendiente de procesar
- templates/ → plantillas base
- resources/ → material de referencia

## Tags principales del sistema
- #daily → notas diarias
- #proyecto → proyectos
- #research → investigaciones
- #persona → contactos
- #idea → ideas sueltas
- #inbox → pendiente de procesar
- #estado/activo, #estado/pausado, #estado/completado → estado de proyectos
- #prioridad/alta, #prioridad/media, #prioridad/baja → urgencia
- #tema/[categoria] → clasificación temática libre

## Reglas de comportamiento
- Si una nota pertenece a un proyecto, enlázala en la sección "🔗 Relacionado" del proyecto
- Si aparece una persona relevante en una nota, crea o enlaza su nota en personas/
- Si una idea madura, conviértela en proyecto usando templates/proyecto.md
- Si algo entra sin contexto, déjalo en inbox/
- Prioriza claridad, conexión entre notas y utilidad futura por sobre exceso de detalle

## Plantillas
Las plantillas usan variables de Obsidian (`{{title}}`, `{{date:YYYY-MM-DD}}`). Cuando crees una nota tú mismo, sustitúyelas por el valor real.

| Tipo de nota | Plantilla | Carpeta |
|---|---|---|
| Nota diaria | templates/daily-note.md | daily-notes/ |
| Proyecto | templates/proyecto.md | proyectos/ |
| Persona | templates/persona.md | personas/ |
| Research | templates/research.md | research/ |

## Seguridad
- Nunca borres notas: si algo sobra, pregúntame primero.
- Lee una nota antes de sobrescribirla; al renombrar o mover, actualiza sus [[enlaces]].
- No toques .obsidian/ ni los archivos binarios (imágenes, pdf, sprites) sin que lo pida.
- proyectos/Proyecto DQ/ es una carpeta de recursos (sprites, pdf) anterior a este sistema: no la reorganices sin preguntar.

## Skills de la bóveda (.claude/skills/)
vault-captura (apuntar rápido) · vault-diario (nota del día) · vault-inbox (procesar inbox/) · vault-nota (crear notas con plantilla) · vault-proyecto (proyectos) · vault-buscar (consultar) · vault-revision-semanal · vault-mantenimiento (auditoría).
