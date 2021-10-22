## Ambiente conda

Se creó un ambiente conda con los paquetes de R utilizados en el curso.

```shell
$ conda update conda
$ conda create -n r
$ conda activate r
$ conda config --env --add channels conda-forge
$ conda config --env --set channel_priority strict
$ conda install r-base r-essentials r-ggplot2 r-plotly r-sf r-terra r-raster r-leaflet r-leaflet.providers r-leaflet.extras r-leaflet.minicharts r-leafem r-flexdashboard r-shiny
```

Se prefirió instalar los paquetes desde la línea de comandos del sistema operativo, como parte del ambiente conda, en lugar de instalarlos desde R mediante `install.packages()`. Aparentemente, así se obtienen mejores resultados.
