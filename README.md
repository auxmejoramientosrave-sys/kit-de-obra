# kit-de-obra
# Kit de arranque — marketplace `kit-arranque`

Marketplace de plugins de Claude con un kit de arranque para gestión documental
y seguimiento de obra.

**Si eres quien lo va a usar, empieza por [EMPIEZA-AQUI.md](EMPIEZA-AQUI.md).**

## Instalación

```
/plugin marketplace add USUARIO/REPO
/plugin install kit-obra@kit-arranque
```

Actualizar más adelante:

```
/plugin marketplace update
```

## Contenido

```
.claude-plugin/marketplace.json     definición del marketplace
plugins/kit-obra/                   el plugin
EMPIEZA-AQUI.md                     guía de arranque para el usuario final
```

| Plugin | Descripción |
|---|---|
| [`kit-obra`](plugins/kit-obra/) | 7 skills (entrevista de arranque, actas, bitácora, informes de avance, control de cambios, gestión documental, herramientas internas) y 1 agente revisor de documentos. |

## Publicar este repositorio

Si acabas de recibir esta carpeta y aún no está en GitHub:

```bash
cd kit-obra
git init
git add .
git commit -m "Kit de arranque para gestión y seguimiento de obra"
git branch -M main
git remote add origin https://github.com/USUARIO/REPO.git
git push -u origin main
```

El repositorio debe ser **público** para que otra persona pueda instalarlo con
`/plugin marketplace add`. Si va a ser privado, quien lo instale necesita acceso
al repositorio.

Antes de publicar, cambiar el campo `owner.name` en
`.claude-plugin/marketplace.json` y `author.name` en
`plugins/kit-obra/.claude-plugin/plugin.json` por quien corresponda.

## Alcance y límites

El kit está escrito con referencias normativas de **Colombia** y prácticas de
obra de ese contexto. Son un punto de partida: en cada proyecto manda el
contrato y la normativa local. Verificar antes de reproducir una cita normativa
en un documento firmado.

Licencia MIT. Úsalo, cámbialo y compártelo.
