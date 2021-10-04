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
    
# Cantones
$ ogr2ogr \
    -t_srs EPSG:4326 \
    -makevalid \
    cantones-wgs84.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limitecantonal_5k"
$ ogr2ogr \
    -t_srs EPSG:5367 \
    -makevalid \
    cantones-crtm05.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limitecantonal_5k"
    
# Distritos
$ ogr2ogr \
    -t_srs EPSG:4326 \
    -makevalid \
    distritos-wgs84.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limitedistrital_5k"
$ ogr2ogr \
    -t_srs EPSG:5367 \
    -makevalid \
    distritos-crtm05.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limitedistrital_5k"
```
