# SHINRAIDEN · Instalador oficial

Instalador del cliente **SHINRAIDEN** para **Minecraft Java 26.2** con **Fabric** y **Java 25**.

### ⬇ Descargar

**[Descargar la última versión](../../releases/latest)** → el archivo `Instalador_SHINRAIDEN.exe`

No hay que descargar nada más de esta página.

---

## Antes de abrirlo

- **Windows 10 u 11, 64 bits.** No hay versión para Mac, Linux ni 32 bits.
- **Minecraft Java 26.2 con Fabric** ya instalado, con una instancia creada, y **Java 25**.
  Funciona con ElyPrismLauncher y con el launcher oficial.
- **Minecraft cerrado.** El instalador comprueba de verdad que no haya archivos bloqueados antes de
  escribir nada.
- Unos **400 MB libres**.

No necesitas instalar .NET: el programa lleva dentro todo lo que necesita. **No necesitas permisos
de administrador**: si algo te los pide, desconfía.

## Windows te avisará la primera vez

Verás **«Windows protegió tu PC»**. Pulsa **Más información → Ejecutar de todas formas**.

Ocurre porque el ejecutable no está firmado con un certificado de pago de Microsoft, no porque tenga
nada malo. Las **actualizaciones** sí van firmadas criptográficamente y el programa las rechaza si la
firma no cuadra.

Puedes comprobar que tu descarga es íntegra comparando su SHA-256 con el que publica
`SHA256SUMS.txt` en la misma release:

```powershell
Get-FileHash .\Instalador_SHINRAIDEN.exe -Algorithm SHA256
```

## Un mod hay que bajarlo a mano

**Freerunner** es obligatorio y su autor reserva todos los derechos, así que no se puede incluir
aquí. El instalador te lo resuelve en la pantalla **CONTENIDO QUE FALTA**: pulsa **ABRIR PÁGINA
OFICIAL**, descarga el archivo y pulsa **IMPORTAR ARCHIVO DESCARGADO**. Es un paso, una vez.

Todo lo demás se descarga y se verifica automáticamente.

## Qué hace y qué no toca

El instalador detecta tu instancia, descarga y comprueba el hash de cada archivo, **hace una copia
recuperable antes de aplicar cambios** y verifica el resultado antes de darlo por bueno. Si algo
falla a mitad, recupera el estado anterior.

**No toca** tus mundos, tus capturas, tu cuenta, tus controles, tu idioma, ni los mods, paquetes o
shaders que hayas puesto tú. Una actualización **no es** una instalación limpia: solo la instalación
limpia retira contenido, y únicamente si la aceptas expresamente de forma explícita.

Tus preferencias y tus copias de seguridad se guardan en `%LOCALAPPDATA%\SHINRAIDEN`. No se escribe
nada en el registro de Windows ni fuera de tu carpeta de usuario.

## Actualizaciones

Abre el instalador y él mismo comprueba si hay una versión nueva. Te muestra el número y los cambios
antes de hacer nada. Hay dos cosas que se actualizan por separado:

- **El programa**: descarga el ejecutable nuevo, comprueba su firma y su hash, lo sustituye y se
  reinicia. Si la versión nueva no arranca, **restaura la anterior**. No cierra Minecraft para
  actualizarse.
- **El contenido** (mods, paquetes, shaders): te presenta el plan de cambios y lo aplica solo si lo
  aceptas.

Conserva el nombre del archivo `Instalador_SHINRAIDEN.exe`: es el que usa para actualizarse.

Sin internet el programa abre y funciona con lo que ya tengas, y te dice con claridad qué no puede
obtener.

## Licencias y autoría

SHINRAIDEN no incluye archivos originales de Mojang. Cada mod, paquete y shader conserva su licencia
y la autoría de quien lo hizo; los que no se pueden redistribuir **no están aquí** y el instalador te
lleva a su fuente oficial.

Los componentes que sí se publican con autorización van listados en el archivo
`REDISTRIBUCION-AVISOS.txt` de cada release, con su autoría y su licencia. **Bountiful** se publica
bajo **LGPL-3.0** como obra derivada del trabajo de Ejektaflex: su código fuente correspondiente se
entrega sin coste a quien lo solicite abriendo una incidencia en este repositorio.

## Problemas frecuentes

| Problema | Solución |
|---|---|
| No encuentra mi instancia | **BUSCAR MANUALMENTE** y selecciona su carpeta |
| Dice que Minecraft está abierto | Ciérralo del todo, incluido el launcher |
| Falta contenido | **CONTENIDO QUE FALTA** → localizar la biblioteca, abrir la página oficial o importar el archivo |
| Quiero deshacer algo | Portada → **RECUPERAR COPIA** |
| Windows bloquea el EXE | **Más información → Ejecutar de todas formas** |
