# Mapas de Campo — visor de mapas sin internet

App: https://cobocuburjosue-glitch.github.io/MAPAS-CAMPO/
Ábrela en Chrome del teléfono ▸ **Instalar app**. Ábrela una vez con internet; después funciona sin señal.

## 1. Mapas sin internet
Los mapas se importan una vez y quedan guardados en el teléfono.

## Región: Guatemala
Coordenadas por defecto en **UTM 15N (WGS 84)**, que cubre todo el país sin saltar a zona 16 al cruzar −90°. También: GTM, UTM 16N, lat/lon decimal y grados-min-seg (toca la barra negra o cámbialo en el botón de capas). Si el GPS da una posición fuera de Guatemala la app avisa y no la usa en los recorridos. El CSV exporta UTM 15N y GTM.

## 2. GPS en tiempo real
Punto azul con flecha de dirección al moverte. La barra inferior muestra coordenadas (toca para cambiar lat/lon ↔ UTM), precisión, altitud, velocidad, rumbo y el valor del ráster donde estás.

## 3. Formatos que se pueden importar
| Formato | Cómo |
|---|---|
| **GeoPDF** (.pdf) | QGIS ▸ Exportar como PDF ▸ marcar “Crear PDF geoespacial”. También ArcGIS/GDAL (formato ISO). |
| **GeoTIFF** (.tif) | Mapas de tasa, índices, ortofotos. 1 banda: muestra el valor al tocar. |
| **JPG/PNG georreferenciado** | Selecciona juntos la imagen + su .jgw/.pgw/.wld (y .prj o .aux.xml si lo tienes), o ponlos en un .zip. |
| **KML / KMZ** | Incluye imágenes superpuestas del KMZ. |
| **GPX**, **GeoJSON** | |
| **Shapefile** | Selecciona juntos .shp + .dbf + .prj (+ .shx), o en .zip. |

## 4. Recorridos
Botón de línea: graba. Calcula distancia, tiempo, velocidad promedio, subida/bajada y elevación mín–máx. Deja la pantalla encendida mientras grabas.

## 5. Placemarks (puntos de interés)
Toca el botón 📍 para activar el **modo Placemark** y luego **toca 2 veces** (o doble clic) donde quieras el punto. También: "En mi posición" o mantener presionado el mapa.
Cada punto guarda: nombre, tipo (árbol, plaga, maleza, trampa, pozo, estación, lindero, muestreo), coordenadas UTM 15N / GTM / lat-lon, fecha y hora, descripción, fotos y atributos (Lote, Finca, Plaga, Incidencia, Responsable…).
- Si el punto cae dentro de un lote de tu KMZ o shapefile, **Lote y Finca se llenan solos**.
- **Fotos georreferenciadas:** cada foto guarda sus propias coordenadas (las de la foto si las trae, o el GPS al tomarla) y la hora. Al exportar se escriben dentro del JPG (EXIF GPS), así QGIS ("Importar fotos geoetiquetadas"), ArcGIS y Google Earth las ubican.

## Compartir el trabajo
Botón ⇪ arriba: **KMZ con fotos**, **KML**, **Excel (CSV)** o **GeoJSON**. El KMZ trae carpetas Puntos, Recorridos y áreas, y Fotos (cada foto en el lugar donde se tomó).

## Abrir archivos con la app
Con la app instalada, en WhatsApp, Archivos o Drive toca **Compartir ▸ Mapas** y el mapa se importa solo. En computadora: clic derecho ▸ Abrir con ▸ Mapas de Campo. Si no aparece la opción, desinstala la app y vuelve a instalarla desde el enlace.

## Otras herramientas
Medir distancia y área (ha), superponer varios mapas, opacidad y colores del ráster.


