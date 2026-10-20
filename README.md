# Calendario de Mentiroso

Calendario mensual público estático, sin dependencias, cuentas de visitantes, analítica ni APIs de pago.

Web: https://mentirosoyoutube.github.io/mentiroso-calendario/

## Datos y mantenimiento

Datos persistentes: juegos.json. Reglas de actualización: AGENTS.md.
Con GitHub conectado, leer ambos archivos en su versión actual y usar el SHA vigente al guardar. Verificar después el archivo y la publicación. Abrir la web no concede permisos de escritura.

Cada juego utiliza id único, name, status selected, releaseDate YYYY-MM-DD y officialUrl HTTPS. Campos opcionales: recordingDate, coverUrl, platforms, releaseType, dateSourceUrl, verifiedAt. Mantener lanzamiento y grabación separados. El calendario muestra lanzamiento y, cuando difiere, la grabación autorizada. Actualizar updatedAt con fecha ISO.

## Publicación

GitHub Pages: Deploy from a branch, main, /(root). Los datos se obtienen al abrir la página; las cachés pueden tardar en reflejar cambios.

## Privacidad

El sitio, el repositorio y su historial son públicos. Solo alojar información autorizada para el calendario. Mantener documentación interna, investigación y datos confidenciales fuera del repositorio. Ocultar enlaces no restringe acceso. La retirada de contenido de la versión actual no borra el historial ni copias previas.
