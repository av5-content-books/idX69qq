# Cartilla de mantenimiento

Un renglón por intervención, en orden. No se borra.

- **Fecha**: `AAAA-MM-DD`.
- **Motivo**: `cotejo`, `reporte del lector`, `drift de plataforma`, `promoción`, `metadatos`, `empaquetado`.
- **Intervención**: qué se hizo y sobre qué archivos, con el alcance real.
- **Estado**: `sano`, `reparado`, `no cotejable`, `pendiente`.
- **Evidencia**: ruta al log, al reporte de EPUBCheck, al diff o al commit. Sin evidencia no vale.

Un ebook ya descargado no se borra sin que el usuario lo pida en ese mismo momento.

| Fecha | Motivo | Intervención | Estado | Evidencia |
| --- | --- | --- | --- | --- |
| 2026-11-10 | metadatos | Se corrigió el título de `BASE/PDF ES idX69qq.pdf` en Info y XMP conforme a la portadilla: «Leyes para todos los días». El texto, los objetos de página y los marcadores coinciden con el original. El PDF se publicó en R2 y su espejo de 421 objetos se verificó por SHA-256 y HTTP 200. | reparado | `.traductor/Metadatos PDF 2026-11-10.json` |
| 2026-11-19 | empaquetado | Revisión del catálogo: el repo no tiene EPUB (origen PDF). Defender no encontró amenazas. | sano | EpubCheck 5.2.1 (`validar_epub.py`) y Microsoft Defender sobre `~/Contraentropia/Producción`, 19/11/2026; resumen en la nota «Mantenimiento a ebooks» del tablero. |
