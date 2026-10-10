# Convención de commits — code-notes

Este repositorio guarda notas en Markdown sobre computación, software y TI.
Los commits se usan como una micro-ficha de estudio: cada uno registra qué se
aprendió y para qué sirve.

## Formato

Seguimos [Conventional Commits](https://www.conventionalcommits.org/):

```
<tipo>(<scope>): <resumen en imperativo, <=50 chars>

Aprendizaje: <concepto|patron|teoria|herramienta|comando|troubleshooting>
Resumen: <qué aprendí / de qué trata>
Aplicacion: <cuándo y para qué me sirve>
```

## Tipos

### Notas (conocimiento)

| Tipo    | Uso                                                        |
| ------- | ---------------------------------------------------------- |
| `note`  | Nueva nota / conocimiento capturado                        |
| `docs`  | Mejora, corrección o ampliación de una nota existente      |
| `chore` | Mantenimiento del repo (estructura, config, `.gitignore`)  |

### Proyectos de código

Cuando el repo contenga proyectos de código, se usa la convención común:
`feat`, `fix`, `refactor`, `perf`, `test`, `build`, `ci`.

## Scope

El `scope` indica el área temática. Se lee el historial de un vistazo:

```
note(linux): comandos de gestión de procesos
note(git): modelo de áreas (working, staging, commit)
note(redes): handshake TCP de tres vías
docs(git): corregir ejemplo de rebase interactivo
feat(cli-tool): agregar parser de argumentos
```

Scopes sugeridos: `git`, `linux`, `redes`, `docker`, `sql`, o el nombre del
proyecto. La lista es abierta: agregá los que necesites.

## Tipos de aprendizaje

El campo `Aprendizaje:` clasifica la nota. Valores actuales:

- `concepto`
- `patron`
- `teoria`
- `herramienta`
- `comando`
- `troubleshooting`

¿Querés agregar uno nuevo? Es solo texto: editá `.github/.gitmessage.txt` y
sumá la opción. No hay validación que se rompa ni commits viejos que migrar.

## Activar la plantilla

La plantilla precarga el borrador del mensaje. Se activa **solo para este repo**
(no toca tu configuración global):

```bash
git config commit.template .github/.gitmessage.txt
```

A partir de ahí, `git commit` (sin `-m`) abre el editor con la plantilla.
Las líneas que empiezan con `#` son guía y Git las descarta al commitear.
