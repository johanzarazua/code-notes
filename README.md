# code-notes

Notas personales en Markdown sobre **computación, software y TI**: conceptos,
patrones, teoría, herramientas, comandos y troubleshooting que voy aprendiendo.

Cada commit funciona como una micro-ficha de estudio: registra *qué* aprendí y
*para qué* sirve, de modo que el historial sea tan útil como las notas mismas.

## Organización

Las notas se agrupan por área temática (el mismo `scope` que uso en los
commits): `git`, `linux`, `redes`, `docker`, `sql`, etc. La estructura va
creciendo a medida que sumo temas.

## Convención de commits

Uso [Conventional Commits](https://www.conventionalcommits.org/) adaptados:

- `note(scope):` — nueva nota / conocimiento capturado
- `docs(scope):` — mejora o corrección de una nota existente
- `chore(scope):` — mantenimiento del repo
- `feat/fix/refactor/...` — proyectos de código dentro del repo

El detalle completo, con la plantilla de commit y los tipos de aprendizaje,
está en [`.github/CONTRIBUTING.md`](.github/CONTRIBUTING.md).

## Ramas

- Notas → directo a `master`.
- Proyectos de código o notas largas en progreso → rama corta
  (`feat/<nombre>`, `note/<tema>`) y merge al terminar.

## Contribuciones

Por ahora es un repositorio **personal** y las contribuciones externas no están
abiertas. Si eso cambia en el futuro, se documentará aquí y en
`.github/CONTRIBUTING.md`.

## Licencia

Las notas y la documentación de este repositorio están bajo
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/):
podés reutilizarlas y adaptarlas siempre que des crédito.

El código fuente que se agregue en carpetas de proyectos queda bajo licencia
**MIT**. Ver el archivo [`LICENSE`](LICENSE).
