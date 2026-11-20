# Seguridad

## Informar de una vulnerabilidad

Por favor, no abras un issue público para un problema de seguridad. Usa *Security → Report a vulnerability* en este repositorio (informe privado de GitHub) y describe lo que has encontrado y cómo reproducirlo.

## Qué hace la app en tu ordenador

- Guarda tus datos solo en `~/.mi_backlog_juegos/`. No hay cuentas, claves ni telemetría.
- Solo se conecta a internet para buscar el nombre del juego que escribes (Steam, HowLongToBeat, Metacritic) y para consultar las Releases de este repositorio en busca de actualizaciones.
- Actualizar el `.exe`: solo descarga por HTTPS el archivo de una Release de este repositorio, comprueba su tamaño, su SHA-256 (también contra el escrito en las notas de la Release) y que es un programa de Windows, y solo entonces se reemplaza. No se instala nada sin tu confirmación.
- El `.exe` no está firmado, así que Windows SmartScreen puede avisar. Puedes comparar el SHA-256 del archivo descargado con el de las notas de la Release.
- Al importar una copia de seguridad se validan todos los nombres de archivo y campos; no se escribe nada fuera de la carpeta de datos.
