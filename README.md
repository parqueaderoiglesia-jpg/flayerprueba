# Generador de flyers Trvely

Arma flyers con vista previa en tiempo real y descarga en PNG (900x1600, formato historia).

## Publicar en GitHub Pages
1. Sube todo el contenido de esta carpeta a un repositorio (rama `main`).
2. En **Settings > Pages**: *Deploy from a branch*, rama `main`, carpeta `/ (root)`.

## Archivos
- `index.html`: la aplicación (4 diseños: Estándar, Oferta, Itinerario, Promo 2x1).
- `datos-trvely.json`: destinos, hoteles y qué incluye cada plan. Al escribir un destino se cargan días, noches, íconos, hotel y mascota.
- `config.json`: diseño vigente. `activa` = plantilla por defecto (`t1` Estándar, `t2` Oferta, `t3` Itinerario, `t4` Promo 2x1). Cada campaña con `desde`/`hasta` (AAAA-MM-DD) cambia la plantilla en esas fechas.

## Imágenes que debes subir (PNG con fondo transparente para logos y mascotas)
- `img/marca/logo-trvely.png`: logo blanco de Trvely.
- `img/hoteles/`: logos en blanco de cada hotel. Los nombres esperados están en el campo `logo` de `datos-trvely.json` (ej. `tamaca.png`, `dubai.png`, `marbelo.png`).
- `img/stickers/`: `caballito-mar.png`, `pulpo.png`, `estrella-mar.png`, `iguana.png`, `tortuga.png`.
- `img/destinos/`: fotos de fondo. Nombres esperados: `playa-palmera.jpg`, `playa-aerea.jpg`, `cartagena-ciudad.jpg`, `medellin.jpg`, `pareja-playa.jpg`, `europa.jpg`. Para agregar más, suma una línea a `BANCO` al inicio del script de `index.html`.
- Usa solo fotos con licencia comercial.

## Guía de marca aplicada
- Colores: Burgundy Travel `#B41241`, Confort Beige `#F4E5D2` y blanco. El verde de las nubes `#0B5E56` y el panel claro `#EFEEE9` salen de los flyers actuales. Se pueden cambiar en el formulario (Marca) y volver a los de marca con un botón.
- Tipografía: la guía define Montserrat (títulos ExtraBold con tracking -5, subtítulos y párrafos Regular/Medium/Bold). Los flyers actuales usan una fuente condensada, por eso el selector ofrece Bebas Neue (como los flyers) y Montserrat ExtraBold (guía), además de Anton y Work Sans.
- Logo: no distorsionar, rotar, aplicar degradados, contornos ni cambiar colores; usar versión blanca sobre fondos oscuros o fotos legibles.

## Pendientes
- Hotel Blue Island está "POR CONFIRMAR" y Poblado Hotel tiene el destino asumido (Coveñas).
- No se guardan precios: se escriben en el formulario.
