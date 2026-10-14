# Datos de cuencas de Manabí

Repositorio de **datos** para la docencia en la Escuela Superior Politécnica Agropecuaria
de Manabí *Manuel Félix López* (ESPAM MFL). Lo usan los cuadernos de varias asignaturas;
aquí no hay cuadernos, solo datos.

Docente responsable: Ing. Cristian Paliz Acosta, MSc. · ORCID 0000-0002-1738-8131

## Cuencas disponibles

Ayampe · Carrizal · Chone · Jama · Jipijapa · Portoviejo

## Cómo se obtienen

Cada cuenca se publica como un archivo ZIP en la sección **Releases**. Dirección directa:

```
https://github.com/crispaliz/datos-manabi/releases/download/<versión>/insumos_<Cuenca>.zip
```

Ejemplo: `https://github.com/crispaliz/datos-manabi/releases/download/v1/insumos_Carrizal.zip`

Los cuadernos de Colab descargan estos archivos solos; no hace falta bajarlos a mano.

## Contenido de cada ZIP

| Carpeta | Archivo | Descripción |
|---|---|---|
| `DEM_Cuencas_Manabi/` | `DEM_<Cuenca>_limpio.tif` | Modelo digital de elevación ALOS PALSAR, 12,5 m, recortado con margen alrededor de la cuenca. UTM 17S (EPSG:32717) |
| `Cuencas_Manabi/` | `cuenca_<Cuenca>.shp` | Límite oficial de la cuenca |
| `Cauces_Manabi/` | `cauce_principal_<Cuenca>.shp` | Cauce principal |
| `Rios_Manabi/` | `rios_dem_<Cuenca>.shp` | Red de drenaje con orden |
| `Suelo_Vegetacion/` | `suelos.shp`, `vegetacion.shp`, `snap.shp` | Suelos, cobertura y áreas protegidas |
| `VIAS-EC/VIAS Y ACCESO/` | `vias z17.shp`, `poblaciones.shp` | Vías y centros poblados |
| raíz | `estaciones_precipitacion.csv` | Estaciones del INAMHI con serie climatológica depurada (filtro de valores atípicos espaciales) |

En la raíz de este repositorio está además `estaciones_precipitacion.csv` con el **catálogo
nacional sin depurar** del INAMHI, que se usa en los ejercicios de control de calidad.

## Versiones

| Versión | Fecha | Cambios |
|---|---|---|
| v1 | octubre de 2026 | Primera publicación: seis cuencas |

Un archivo publicado en una versión **no se reemplaza**: cualquier corrección se publica como
una versión nueva, para que los cuadernos de cada semestre sigan funcionando.

## Fuentes

Modelo digital de elevación ALOS PALSAR (12,5 m). Capas base de fuentes oficiales
ecuatorianas. Estaciones meteorológicas del Instituto Nacional de Meteorología e
Hidrología (INAMHI). Uso académico: cita las fuentes originales en tus trabajos.
