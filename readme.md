# Claude Board

Tablero local para ver qué hacen tus agentes de Claude Code, en todos tus proyectos a la vez: qué sesiones están trabajando, cuáles esperan un permiso y cuánto consume cada una.

> Proyecto independiente y no oficial. No está afiliado ni respaldado por Anthropic. "Claude" y "Claude Code" son marcas de Anthropic.

## Instalar

1. Entra a [Releases](../../releases/latest) y descarga el archivo `Claude-Board_X.Y.Z_x64-setup.exe`.
2. Ábrelo. Se instala solo para tu usuario, sin permisos de administrador.
3. Abre Claude Board, ve a **Ajustes → Hooks** y pulsa **Instalar hooks**. Después reinicia las sesiones abiertas de Claude Code.

Requiere Windows 10 u 11 (x64). Si falta WebView2, el instalador lo descarga y necesita internet en ese momento.

> Es posible que Windows o tu antivirus muestren un aviso al abrir el instalador, porque todavía no está firmado con un certificado de Windows. Puedes comprobar que el archivo es el original con su SHA-256 (ver más abajo).

## Actualizar

Desde la propia app: **Ajustes → Actualizar → Buscar actualizaciones**. Las actualizaciones vienen firmadas y la app rechaza cualquiera que no coincida con la firma del proyecto.

## Comprobar la descarga

Cada release incluye un archivo `.sha256`. En PowerShell:

```powershell
Get-FileHash .\Claude-Board_X.Y.Z_x64-setup.exe -Algorithm SHA256
```

El resultado debe coincidir con el del `.sha256` de ese release.

## Privacidad

Todo es local: tu actividad no se envía a internet. La única conexión de la app es la consulta de actualizaciones a este repositorio, y solo cuando pulsas **Buscar actualizaciones**.

## Licencia

Software propietario, todos los derechos reservados. Puedes instalarlo y usarlo para ti o tu equipo; no puedes redistribuirlo, modificarlo ni aplicarle ingeniería inversa sin permiso por escrito. El código fuente no se publica. Se ofrece sin garantía.

Hecho por [KuroNeko](https://github.com/imkuroneko).
