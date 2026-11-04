# Talonario web

Aplicación web estática en español para diseñar talones, generar folios correlativos y preparar la impresión en hojas A4. No requiere instalar dependencias ni tener un servidor de aplicación.

## Abrir

Abre `index.html` con un navegador moderno. Para imprimir o cargar imágenes y proyectos, permite al navegador acceder a archivos locales.

## Funciones

- Imagen de fondo o fondo en blanco y área de diseño de proporción 10:3 o ajustada a la imagen.
- Veintitrés fondos de ejemplo listos para usar, incluidos en la carpeta `fondos/`.
- Textos y folios arrastrables, con 30 opciones de tipografía, tamaño, color, negrita y cursiva. La disponibilidad visual de algunas fuentes depende del sistema operativo.
- Formas vectoriales insertables (línea, flecha, rectángulo, triángulo y elipse), movibles, redimensionables y editables en color, grosor en píxeles de diseño, trazo punteado y relleno; se conservan en proyectos y al imprimir.
- Los controles del elemento seleccionado aparecen debajo del área de diseño para editarlos sin apartarse del talón; cualquier elemento se puede mover una capa adelante o atrás, o directamente al frente o al fondo.
- Los objetos se pueden ocultar y volver a mostrar desde sus controles, incluido el folio principal.
- Folios consecutivos con número inicial, cantidad y prefijo opcional.
- QR opcional y elementos de imagen superpuestos, que se pueden mover, redimensionar y ordenar.
- Biblioteca de 37 decoraciones en el lateral derecho, con motivos infantiles, escolares, festivos, animales, música y deportes; los adornos se pueden insertar con un clic o cargar imágenes propias. Las decoraciones agregadas quedan guardadas dentro del proyecto.
- Carpeta `decoraciones/` organizada por tipo (`infantiles/`, `escolares/`, `fiestas/`, `naturaleza/`, `simbolos/`, `animales/`, `musica/`, `deportes/`, `temporadas/` y `marcos/`) con 27 imágenes SVG listas para usar. La biblioteca de la aplicación ofrece 37 diseños y permite filtrarlos por categoría.
- Rotación de textos, folios, códigos QR e imágenes con un control de -180° a 180°; el ángulo se conserva al guardar, abrir e imprimir proyectos.
- Tamaño de impresión estándar (183,3 × 55 mm) o personalizado, una o dos columnas.
- Vista de distribución A4, marcas de corte en L en el perímetro y en T entre filas de talones, y vista previa/impresión del navegador.
- Guardado y apertura de proyectos `.json`; las imágenes se incluyen dentro del archivo. En navegadores compatibles, Guardar permite elegir la ubicación; en los demás, descarga el archivo.

## Notas

- El proyecto se guarda en el dispositivo desde el que se usa; esta versión no tiene cuentas ni almacenamiento en línea.
- Los fondos de ejemplo se guardan como referencia a `fondos/`; conserva esa carpeta junto a `index.html` para que sigan disponibles. Las imágenes propias sí quedan incorporadas en el archivo del proyecto.
- Para usar una imagen SVG de `decoraciones/`, selecciónala con **Subir imagen propia**. En la biblioteca, usa **Tipo de decoración** para filtrar los adornos por categoría.
- La generación del QR usa `api.qrserver.com`, como la rutina VB.NET original. El texto o URL del QR se envía a ese servicio y se necesita conexión a internet para generarlo.
- La impresión depende de las opciones del navegador y de la impresora. En el diálogo de impresión, selecciona papel A4, orientación vertical y escala 100%; desactiva encabezados y pies de página si el navegador los agrega.
