# Formato de Entrega de Mercancía – IMC Cargo

Formulario web autocontenido (HTML + JS + CSS) para registrar la entrega/recepción de mercancía entre IMC Cargo International SAS y SERVICIOS (Impresistem), con:

- Consecutivo automático (IMC-DDMMYYYY-###)
- Tabla de ítems editable (referencia, descripción, cantidad, serial)
- Verificaciones (cantidad, seriales, evidencia fotográfica)
- Firmas digitales por canvas (4 firmas: entrega/recibe IMC y SERVICIOS)
- Exportación a Excel (SheetJS)
- Sincronización con Google Drive vía Google Apps Script (pestaña "Archivos Drive")

## Archivos

- `index.html` — Aplicación completa (única página)
- `logo-imc.png` — Logo IMC Cargo
- `logo-imp.png` — Logo Impresistem (SERVICIOS)

## Publicar en GitHub Pages

1. Sube estos 3 archivos a la raíz del repositorio (o a una carpeta, ej. `/docs`).
2. En el repo: **Settings → Pages → Source** → selecciona la rama (`main`) y la carpeta (`/root` o `/docs`).
3. Guarda. La URL quedará como `https://<usuario>.github.io/<repo>/`.

## Notas

- El backend de Google Apps Script (`SCRIPT_URL` en el `<script>`) debe quedar publicado como "Cualquier usuario, incluso anónimo" para que el guardado y la sincronización con Drive funcionen desde GitHub Pages.
- Los logos se cargan por nombre relativo (`logo-imc.png`, `logo-imp.png`), así que deben estar en la **misma carpeta** que `index.html`.
