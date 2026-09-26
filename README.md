# Prime Copy · web

Página de presentación de Prime Copy (trade copier para NinjaTrader 8).

Sitio estático: un solo `index.html`, sin build ni dependencias. Se publica tal cual en
Netlify, Cloudflare Pages o GitHub Pages.

Contacto actual: Telegram https://t.me/mrbenitofx

## Imagen de vista previa

`og-image.png` (1200×630) es la imagen que muestran Telegram, WhatsApp y X al compartir el
link. Su diseño está en `og/og.html`. Para regenerarla después de editarlo (PowerShell):

```powershell
& "${env:ProgramFiles(x86)}\Microsoft\Edge\Application\msedge.exe" --headless=new --disable-gpu --hide-scrollbars --force-device-scale-factor=1 --window-size=1200,630 --virtual-time-budget=6000 "--user-data-dir=$env:TEMP\pc-og-profile" "--screenshot=$PWD\og-image.png" "file:///$($PWD -replace '\','/')/og/og.html"
```
