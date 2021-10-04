```shell
# Provincias
$ ogr2ogr \
    -t_srs EPSG:4326 \
    -makevalid \
    provincias.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limiteprovincial_5k"
```
