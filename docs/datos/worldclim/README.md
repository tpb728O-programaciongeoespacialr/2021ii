```shell
# Descarga y descompresión del archivo con datos de altitud para todo el mundo
$ wget https://biogeo.ucdavis.edu/data/worldclim/v2.1/base/wc2.1_30s_elev.zip
$ unzip wc2.1_30s_elev.zip

# Altitud para Costa Rica
$ gdalwarp \
    -dstnodata -9999 \
    -tr 0.008333333333333 0.008333333333333 \
    -q \
    -cutline provincias.shp \
    -crop_to_cutline wc2.1_30s_elev.tif \
    altitud.tif
```
