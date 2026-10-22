# Qué hay y qué no hay en este repositorio

Este repositorio es **público** y existe con un único fin: alojar las **publicaciones** del
instalador SHINRAIDEN para que el propio programa pueda comprobar y descargar sus actualizaciones
sin pedirle credenciales a nadie.

## Qué contiene

- Este texto y el `README.md`.
- Las **Releases**, y dentro de cada una: el ejecutable `Instalador_SHINRAIDEN.exe`, el manifiesto
  firmado `update-manifest.json`, su copia legible `modpack-manifest.json`, los avisos de
  redistribución `REDISTRIBUCION-AVISOS.txt`, las sumas `SHA256SUMS.txt` y los archivos de los
  componentes cuya redistribución está expresamente autorizada.

## Qué NO contiene, y no contendrá

- El **código fuente** del instalador: vive en un repositorio privado del propietario.
- La **clave privada** con la que se firman las actualizaciones. Nunca sale del equipo del
  propietario y no está en ningún repositorio, ni como secret de integración continua.
- Mods, paquetes de recursos o shaders **sin permiso de redistribución** — entre otros Freerunner,
  BSL, Complementary Reimagined, Patrix y Marked Hoppers. El instalador lleva a cada jugador a la
  fuente oficial de su autor o le deja importar su propio archivo.
- Archivos originales de **Mojang**.
- Mundos, cuentas, tokens, configuraciones personales ni copias de seguridad de nadie.
- Componentes exclusivos del servidor.

## Integridad de las descargas

Cada release publica `SHA256SUMS.txt`. El instalador, además, no acepta una actualización cuyo
manifiesto no esté firmado con la clave del propietario, cuyos hashes no coincidan, cuya versión no
sea posterior a la instalada o que no proceda de este repositorio.

## Atribución

Cada componente redistribuido conserva sus bytes originales, su licencia y la autoría de quien lo
hizo. `REDISTRIBUCION-AVISOS.txt`, dentro de cada release, los lista uno por uno. SHINRAIDEN no
reclama la autoría de trabajo ajeno ni cambia la licencia de nadie.

Si eres autor de algo publicado aquí y quieres que se retire, abre una incidencia: se retirará.
