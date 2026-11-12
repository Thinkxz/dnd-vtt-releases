# DND VTT

Una mesa virtual casera para jugar rol con amigos: mapa visto desde arriba, fichas, dados y chat. Es un proyecto personal hecho para un grupo chico; se comparte tal como está, sin soporte.

Acá se publican solo las versiones para descargar.

## Descargar

Bajá el archivo `.zip` de la **[última versión](https://github.com/Thinkxz/dnd-vtt-releases/releases/latest)**.

Funciona en Windows 10 y Windows 11.

## Instalar

No hay instalador.

1. Descomprimí el zip en una carpeta, por ejemplo en `Documentos`. No la abras desde dentro del zip.
2. Entrá a la carpeta `DND VTT` y abrí **DND VTT.exe**.

La primera vez, Windows puede mostrar un cartel azul que dice "Windows protegió tu PC". Aparece porque la app no tiene un certificado pago, no porque haya detectado algo. Tocá **Más información** y después **Ejecutar de todas formas**.

Windows también puede preguntar si la app puede usar la red: marcá **Redes privadas** y aceptá.

## Jugar por internet

La app no usa servidores propios: uno del grupo abre la mesa en su PC y los demás se conectan a esa PC. Para llegar a ella por internet sin tocar el router, todos usan [Tailscale](https://tailscale.com/) (gratis para grupos chicos).

1. Instalá Tailscale e iniciá sesión.
2. Pedile a quien abre la mesa que te sume a su red y te pase la **invitación**.
3. En la app, pegá la invitación en "Unirse".

## Actualizar

La app avisa cuando hay una versión nueva. Para actualizar, bajá el zip nuevo y descomprimilo en otra carpeta; la anterior la podés borrar.

Tu perfil y tus partidas guardadas no están dentro de la carpeta de la app, así que no se pierden.

Si la app dice que tu versión es más vieja que la de la mesa, hay que actualizar para poder entrar.

Las versiones de prueba se publican como "Pre-release": la app no las anuncia y no hace falta bajarlas.

## Comprobar la descarga (opcional)

Cada versión publica el tamaño y la huella SHA-256 de su zip. Para ver la huella del archivo que bajaste, abrí PowerShell en esa carpeta y escribí:

```powershell
Get-FileHash .\DND-VTT-*.zip -Algorithm SHA256
```

Tiene que coincidir con la que figura en la página de esa versión.

## Qué hace la app en internet

- Consulta este repositorio para saber si hay una versión nueva.
- Se conecta a la PC de quien abrió la mesa, por la red privada que eligieron.

No manda datos a ningún otro lado y no tiene cuentas ni registro.

## Créditos y licencias

La app usa Electron, Three.js y Colyseus, fuentes de licencia libre y contenido del SRD de D&D 5e bajo licencia CC-BY-4.0. El detalle y las atribuciones están en `CREDITOS.txt`, dentro del zip.

El zip incluye el código de esa versión en forma legible.
