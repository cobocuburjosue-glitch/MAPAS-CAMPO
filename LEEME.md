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

## 5. Puntos de interés
Mantén presionado el mapa o toca 📍 (en tu posición). Tipos: árbol, plaga, maleza, trampa, pozo, estación meteorológica, lindero, sitio de muestreo, otro. Cada punto lleva nombre, descripción, fotos (cámara o galería), coordenadas lat/lon y UTM, y atributos personalizados (la app recuerda los atributos que usaste por tipo).

## Exportar
Botón capas ▸ Exportar: **KMZ con fotos** (Google Earth / QGIS), **CSV** (Excel, con UTM y atributos) o **GeoJSON**. Se puede compartir directo por WhatsApp o correo.

## Otras herramientas
Medir distancia y área (ha), superponer varios mapas, opacidad y colores del ráster.


