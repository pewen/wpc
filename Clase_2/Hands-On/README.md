# Hands-On Numpy y Matplolib

## Agua o tierra

Escriba un programa que tome coordenadas geográficas como entrada e imprima si esa coordenada es tierra o agua. El programa debe ser usado como un pipe de la linea de comandos.

**Tip:**
* [numpy.fromfile](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fromfile.html)
* El archivo *data/gl-latlong-1km-landcover.bsq.bz2* es un binario que contiene de, de forma codificada, si la posición que consultamos es agua o tierra. El archivo *data/gl0500bs.txt* posee características de este binario.

Los datos se extrajeron de: http://www.landcover.org/data/landcover/

### Eventos

Por cada evento que hay en el archivo *data/events.txt*, agregarle una columna al final indicando si ocurrió en agua o tierra.

### Graficando

Por cada evento que el usuario pasa por linea de comando o mediante un archivo de texto, marcarlo con un cuadrado sobre el mapa *data/gl-latlong-1km-landcover.preview.jpg*. Si el evento ocurrió sobre agua, que el cuadrado sea de color azul. Caso contrario de color rojo.


## Datos faltantes

Muchos archivos de datos poseen el siguiente formato:

```
fecha inicial - fecha final
datos
dato faltante
mas texto
```

Escribir un script en python que reciba una archivo de este tipo (*data/nina3.data*), y retorne una matriz remplazado los valores faltantes por NaN.

**Tips:**
* Para la lectura de este tipo de archivo, se puede utilizar [numpy.fromfile](https://docs.scipy.org/doc/numpy/reference/generated/numpy.fromfile.html) o de la biblioteca Pandas, [from_csv](http://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_csv.html)

## Promedio

Calcular los promedio y desviación standar por mes y por año.

### Graficar

Graficar estos datos usando matplotlib (histograma, precipitación vs mes).
