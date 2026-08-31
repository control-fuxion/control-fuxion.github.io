# Respaldo automático FuXion

Este directorio conserva copias **cifradas** de FuXion Studio y Mi Control FuXion.

- Se crea una copia automática cada 24 horas, aproximadamente a las 00:20 de Lima.
- Se conservan los últimos 35 días.
- `latest.fxbackup` contiene la copia más reciente.
- `data/AAAA-MM-DD/` contiene el historial diario.
- Ningún archivo puede abrirse sin `CLAVE-RECUPERACION-FUXION.txt`.

Para abrir una copia, visita `https://control-fuxion.github.io/recovery/`. El descifrado ocurre únicamente dentro del navegador y no envía la clave ni los datos a un servidor.

El código de las páginas permanece protegido por el historial de versiones de las dos publicaciones activas.
