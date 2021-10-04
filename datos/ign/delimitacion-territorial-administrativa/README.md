```shell
# Provincias
$ ogr2ogr \
    -t_srs EPSG:4326 \
    -makevalid \
    provincias-wgs84.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limiteprovincial_5k"
$ ogr2ogr \
    -t_srs EPSG:5367 \
    -makevalid \
    provincias-crtm05.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limiteprovincial_5k"    
```
