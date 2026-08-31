# Código de recuperación de las páginas FuXion

Esta copia conserva el código de **FuXion Studio de Yair** y **Mi Control FuXion** publicado el 31 de agosto de 2026. No incluye contraseñas, claves privadas ni datos de clientes.

El archivo comprimido se dividió en partes de texto para conservarlo en GitHub. Para reconstruirlo en Windows PowerShell, abre esta carpeta descargada y ejecuta:

```powershell
$partes = Get-ChildItem "fuxion-sites-source-2026-08-31.tar.gz.b64.part*" | Sort-Object Name
$base64 = ($partes | ForEach-Object { Get-Content $_.FullName -Raw }) -join ""
[IO.File]::WriteAllBytes("fuxion-sites-source-2026-08-31.tar.gz", [Convert]::FromBase64String($base64))
```

SHA-256 esperado:

`4246c46d24a267fbe9238f9d06f2a8f7ba41d1e22383ccb198b66a60216cf28f`
