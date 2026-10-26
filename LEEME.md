# Mapas de Campo — visor de mapas sin internet

## Instalar en el teléfono (una sola vez, con internet)
1. Crea un repositorio en GitHub (ej. `MAPAS-CAMPO`) y sube **todos** los archivos de esta carpeta.
2. En el repo: **Settings ▸ Pages ▸ Branch: main / root ▸ Save**.
3. Abre en Chrome del teléfono: `https://<tu-usuario>.github.io/MAPAS-CAMPO/`
4. Toca **Instalar app** (o menú ⋮ ▸ *Agregar a pantalla principal*). Acepta el permiso de ubicación.

Desde ahí la app abre sin señal. Los mapas se guardan solo en ese teléfono.

## Formatos
- **GeoTIFF** (.tif): mapas de tasa, índices, ortofotos. Detecta UTM 15N/16N, WGS84 y GTM; si no trae proyección, te pregunta.
  - 1 banda → colores + valor del píxel al tocar el mapa y bajo tu posición GPS.
  - RGB → se muestra como imagen.
- **KML / KMZ** (incluye imágenes superpuestas del KMZ), **GeoJSON**, **GPX**
- **Shapefile**: comprime .shp + .dbf + .shx + .prj en un **.zip**.

## Uso
- Toca el mapa: valor del ráster en ese punto. Toca la barra negra inferior: cambia entre lat/lon y UTM.
- Mantén presionado el mapa: nueva marca. Botón 📍: marca en tu posición.
- Botón de recorrido: graba tu trayecto (deja la pantalla encendida).
- Botón regla: mide distancia y área (ha).
- Botón capas: opacidad, colores, fondo satelital (con internet), superponer otros mapas, exportar marcas a KML/GeoJSON.

## Consejo para QGIS
Exporta rásters grandes recortados al área de trabajo; la app reduce a ~2200 px (1 banda) o ~3200 px (RGB) por lado para que el teléfono los maneje con fluidez.
