# Calendario de Mentiroso

Calendario público estático para GitHub Pages. Sin dependencias, cuentas de visitantes, analítica ni APIs de pago. No incluye juegos hasta que Daniel los autorice.

## Publicación

Repositorio: https://github.com/MentirosoYoutube/mentiroso-calendario

Datos persistentes: `juegos.json`. Reglas de autorización: `AGENTS.md`.
En Settings → Pages: Deploy from a branch → `main` → `/(root)` → Save.
Dirección del calendario (comprobar despliegue antes de darlo por publicado): https://mentirosoyoutube.github.io/mentiroso-calendario/

## Actualización desde otro chat

Con GitHub conectado, abrir este repositorio y leer `AGENTS.md` y la versión actual de `juegos.json`. Actualizar el archivo mediante el conector, usando su SHA actual, y comprobar después la lectura y la web. La URL por sí sola no concede permisos de escritura.

Los juegos se guardan en `juegos.json`, junto al código, en GitHub; no en localStorage. La web pide los datos al abrirse. La publicación y sus cachés pueden tardar en reflejar un cambio; no darlo por desplegado sin verificarlo.

## Datos

Cada juego seleccionado necesita `id` único, `name`, `status: "selected"`, `releaseDate` (YYYY-MM-DD) y `officialUrl` HTTPS. Opcionales: `recordingDate` (fecha o null), `coverUrl` HTTPS, `platforms` (lista), `releaseType`, `dateSourceUrl`, `verifiedAt`. Al modificar datos, actualizar `updatedAt` a fecha ISO con zona.

El juego aparece siempre en su lanzamiento. Si se autoriza una grabación en otro día, aparece también ese día con etiqueta GRABACIÓN; no se cambia el lanzamiento. La vista del día muestra ambas fechas.

## Investigación

La investigación propone y Daniel elige. Revisar semana siguiente de lunes a domingo, oportunidades restantes de la semana actual, últimos siete días y vigilancia de las dos semanas posteriores. Catálogo amplio verificado más tres candidatos. Distinguir juegos completos, acceso anticipado, demos, expansiones, actualizaciones, remasters y ports. No hay automatización activada por este proyecto.
