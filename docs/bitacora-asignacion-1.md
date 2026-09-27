# Bitácora - Asignación 1

## Tarea 1: Generar el .gitignore para C#

**Qué pedí:**
"Genera un .gitignore correcto para C# con todas las carpetas y archivos que no debo versionar"

**Qué devolvió:**
Claude generó un .gitignore completo con:
- bin/, obj/, Debug/, Release/
- .vs/, .vscode/
- *.dll, *.exe, *.pdb
- .env
- etc.

**Error encontrado y corrección:**
Claude olvidó incluir `appsettings.*.json` (archivos de configuración por ambiente) en la lista. Lo detecté cuando revisé manualmente cuáles archivos generados no deberían estar en el repo. Lo corregí agregando manualmente esa línea al .gitignore.

---

## Tarea 2: Estructura de proyecto C#

**Qué pedí:**
"Crea una estructura base para un proyecto de C#"

**Qué devolvió:**
Sugerencias para crear carpetas src/, docs/, y Program.cs

**Error encontrado y corrección:**
La sugerencia inicial no incluía un .gitkeep en la carpeta docs/ (para preservar carpetas vacías). Lo agregué manualmente después de crear la estructura.