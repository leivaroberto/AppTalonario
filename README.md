# Talonario web

Aplicación web estática en español para diseñar talones, generar folios correlativos y preparar la impresión en hojas A4. No requiere instalar dependencias ni tener un servidor de aplicación.

## Abrir

Abre `index.html` con un navegador moderno. Para imprimir o cargar imágenes y proyectos, permite al navegador acceder a archivos locales.

## Funciones

- Seis plantillas completas, editables e imprimibles: rifa solidaria, cumpleaños, bingo, evento escolar, comida solidaria y concierto. Se eligen desde el botón **Plantillas** en una ventana aparte; cada una incluye un fondo propio y numeración duplicada.
- Imagen de fondo o fondo en blanco; el fondo se puede arrastrar dentro del recuadro para elegir el recorte y se mantiene sin deformarse. El área puede usar proporción 10:3 o ajustarse a la imagen.
- Veintinueve fondos de ejemplo listos para usar, incluidos en la carpeta `fondos/`.
- Textos y folios arrastrables, con 30 opciones de tipografía, tamaño, color, negrita y cursiva. La disponibilidad visual de algunas fuentes depende del sistema operativo.
- Formas vectoriales insertables (línea, flecha, rectángulo, triángulo, elipse y estrella), movibles, redimensionables y editables en color, grosor en píxeles de diseño, trazo punteado y relleno; se conservan en proyectos y al imprimir.
- Los controles del elemento seleccionado aparecen debajo del área de diseño para editarlos sin apartarse del talón; cualquier elemento se puede mover una capa adelante o atrás, o directamente al frente o al fondo.
- Los objetos se pueden ocultar y volver a mostrar desde sus controles, incluido el folio principal.
- Folios consecutivos con número inicial, cantidad y prefijo opcional.
- QR opcional y elementos de imagen superpuestos, que se pueden mover, redimensionar manteniendo su proporción y ordenar.
- Búsqueda integrada de imágenes en Wikimedia Commons para utilizarlas como fondo o imagen superpuesta; la imagen descargada se incorpora al proyecto.
- Biblioteca de 37 decoraciones en el lateral derecho, con motivos infantiles, escolares, festivos, animales, música y deportes; los adornos se pueden insertar con un clic o cargar imágenes propias. Las decoraciones incluidas se guardan como referencia a su archivo en `decoraciones/`, por lo que un proyecto `.json` que las use debe abrirse junto a esa carpeta.
- Carpeta `decoraciones/` organizada por tipo (`infantiles/`, `escolares/`, `fiestas/`, `naturaleza/`, `simbolos/`, `animales/`, `musica/`, `deportes/`, `temporadas/` y `marcos/`) con 27 imágenes SVG listas para usar. La biblioteca de la aplicación ofrece 37 diseños y permite filtrarlos por categoría.
- Rotación de textos, folios, códigos QR e imágenes con un control de -180° a 180°; el ángulo se conserva al guardar, abrir e imprimir proyectos.
- Tamaño de impresión estándar (183,3 × 55 mm) o personalizado, una o dos columnas.
- Vista de distribución A4, marcas de corte en L en el perímetro y en T entre filas de talones, y vista previa/impresión del navegador.
- Guardado y apertura de proyectos `.json`; las imágenes se incluyen dentro del archivo. En navegadores compatibles, Guardar permite elegir la ubicación; en los demás, descarga el archivo.
- Deshacer y rehacer hasta 50 cambios, con botones y atajos `Ctrl+Z`, `Ctrl+Y` o `Ctrl+Mayús+Z`.
- Guardado automático del borrador en el almacenamiento local del navegador y recuperación al volver a abrir la aplicación.

## Notas

- El proyecto se guarda en el dispositivo desde el que se usa; esta versión no tiene cuentas ni almacenamiento en línea.
- El borrador automático se almacena localmente mediante IndexedDB; no reemplaza la descarga de proyectos `.json` para hacer copias o trasladarlos a otro dispositivo.
- Los fondos de ejemplo se guardan como referencia a `fondos/`; conserva esa carpeta junto a `index.html` para que sigan disponibles. Las imágenes propias sí quedan incorporadas en el archivo del proyecto.
- Para usar una imagen SVG de `decoraciones/`, selecciónala con **Subir imagen propia**. En la biblioteca, usa **Tipo de decoración** para filtrar los adornos por categoría.
- La generación del QR usa `api.qrserver.com`, como la rutina VB.NET original. El texto o URL del QR se envía a ese servicio y se necesita conexión a internet para generarlo.
- La búsqueda de imágenes envía el término a Wikimedia Commons y requiere conexión a internet. Se incorpora una versión reducida de hasta aproximadamente 640 píxeles de ancho; para impresiones grandes, descarga el original y cárgalo como imagen de fondo o **Imagen superpuesta**. Antes de usar una imagen, consulta su ficha para conocer su licencia y las condiciones de atribución.
- La impresión depende de las opciones del navegador y de la impresora. En el diálogo de impresión, selecciona papel A4, orientación vertical y escala 100%; desactiva encabezados y pies de página si el navegador los agrega.
