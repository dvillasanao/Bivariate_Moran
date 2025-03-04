
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Análisis de Correlaciones Espaciales Bivariadas

Este repositorio contiene el código y los resultados del análisis de
correlaciones espaciales bivariadas utilizando el **Índice de Calidad
del Entorno (ICE)** en contraste con otros indicadores socioeconómicos
clave:

- **Índice de Marginación (IM)**
- **Índice de Equipamiento (IE)**
- **Índice de Accesibilidad (IA)**

El objetivo es identificar patrones espaciales y relaciones entre estos
indicadores a nivel municipal mediante técnicas de estadística espacial.

<div style="display: flex; justify-content: center;">

<img src="Output/Mapa LISA Cluster_IE.png" width="75%" style="margin: 1px;">

</div>

## Contenido del repositorio

- **`Bases/`**: Datos geoespaciales y tabulares utilizados en el
  análisis.
- **`R/`**: Código en R para calcular correlaciones espaciales.
- **`Output/`**: Salidas de los modelos y mapas generados.

## Metodología

Se utilizaron los siguientes métodos de análisis espacial:

### **1. Índice de Moran Bivariado Global**

Evalúa la autocorrelación espacial entre dos variables en toda la región
de estudio.

### **2. Índice de Moran Bivariado Local (LISA)**

Permite identificar clusters espaciales de alta o baja correlación entre
`ICE` y cada uno de los otros índices.

### **3. Índice de Geary Bivariado**

Mide la heterogeneidad espacial y discontinuidades en la distribución de
los indicadores.

## Enlace

**Enlace**:
<https://dvillasanao.github.io/Bivariate_Moran/Output/Bivariate-Moran-Index.html>  
**Enlace Mapas**:
<https://dvillasanao.github.io/Bivariate_Moran/Output/Mapas.html>

## Requisitos

Para ejecutar el análisis es necesario contar con **R** y las siguientes
librerías:

``` r
install.packages(c("sf", "spdep", "ggplot2", "ggspatial", "dplyr", "purrr"))
```

## Referencias

- Instituto Nacional de Estadística y Geografía (2021). Censo Nacional
  de Población y Vivienda 2020. México: INEGI.
- Secretaría General del Consejo Nacional de Población. (2023). Índices
  de marginación 2020.
  <https://www.gob.mx/conapo/documentos/indices-de-marginacion-2020-284372>
- Consejo Nacional de Población, Instituto Mexicano del Transporte y
  Centro de Investigación en Ciecias de Información Geoespacial. (2023).
  Análisis geoespacial de la accesibilidad a centros urbanos de las
  localidades de México.
  <https://www.gob.mx/conapo/documentos/analisis-geoespacial-de-la-accesibilidad-a-centros-urbanos-de-las-localidades-de-mexico>.
- Secretaría General del Consejo Nacional de Población (2023). Índice de
  Calidad del Entorno 2020. México: CONAPO.
- Secretaría de Desarrollo Social (2012). Sistema Normativo de
  Equipamiento. México: SEDESOL.

## Código de Conducta

Por favor, revisa el [Código de Conducta](CODE_OF_CONDUCT.md) antes de
contribuir.

## Licencia

Este trabajo de Diana Villasana Ocampo está bajo una
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
Licencia Creative Commons Atribución 4.0 Internacional.</a>.
