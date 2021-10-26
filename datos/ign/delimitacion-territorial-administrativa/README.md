```shell
# Provincias
$ ogr2ogr \
    -makevalid \
    provincias.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limiteprovincial_5k"
    
# Provincias simplificadas (100 m)
$ ogr2ogr \
    -simplify 100 \
    -makevalid \
    provincias-simplificadas_100m.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limiteprovincial_5k"   
    
# Cantones
$ ogr2ogr \
    -makevalid \
    cantones.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limitecantonal_5k"
    
# Distritos
$ ogr2ogr \
    -makevalid \
    distritos.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:limitedistrital_5k"
```
