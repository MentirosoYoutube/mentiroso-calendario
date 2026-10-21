# Calendario de Mentiroso

Calendario mensual público estático, sin dependencias, cuentas de visitantes, analítica ni APIs de pago.

Web: https://mentirosoyoutube.github.io/mentiroso-calendario/

## Datos y mantenimiento

Datos persistentes: juegos.json. Reglas de actualización: AGENTS.md.
Con GitHub conectado, leer ambos archivos en su versión actual y usar el SHA vigente al guardar. Verificar después el archivo y la publicación. Abrir la web no concede permisos de escritura.

Cada juego utiliza id único, name, status selected o candidate, releaseDate YYYY-MM-DD y officialUrl HTTPS. Campos opcionales: recordingDate, coverUrl, platforms, releaseType, dateSourceUrl, verifiedAt. candidate indica un lanzamiento en observación, sin compromiso de grabación; selected conserva las selecciones anteriores. Mantener lanzamiento y grabación separados. El calendario muestra lanzamiento y, cuando difiere, la grabación autorizada. Actualizar updatedAt con fecha ISO.

## Publicación

El pie muestra la última modificación de datos y la próxima revisión prevista. `researchSchedule` en juegos.json refleja el horario público verificado de la revisión: `enabled`, `timeZone` IANA, `weekdays` (0 domingo–6 sábado), `hour`, `minute` y `startsOn` YYYY-MM-DD. La web calcula la siguiente fecha al abrir y cada 30 segundos, respetando el huso y los cambios de horario. Este dato no crea ni ejecuta una tarea; si su horario cambia o se pausa, sincronizar esta configuración con el horario real. La revisión propone juegos y no los incorpora automáticamente.

GitHub Pages: Deploy from a branch, main, /(root). Los datos se obtienen al abrir la página; las cachés pueden tardar en reflejar cambios.

## Privacidad

El sitio, el repositorio y su historial son públicos. Solo alojar información autorizada para el calendario. Mantener documentación interna, investigación y datos confidenciales fuera del repositorio. Ocultar enlaces no restringe acceso. La retirada de contenido de la versión actual no borra el historial ni copias previas.

