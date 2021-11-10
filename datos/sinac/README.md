```shell
# Áreas silvestres protegidas
$ ogr2ogr \
    -makevalid \
    areas-silvestres-protegidas.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:areas_silvestres_protegidas"

# Áreas silvestres protegidas simplificadas
$ ogr2ogr \
    -simplify 100 \    
    -makevalid \
    areas-silvestres-protegidas-simplificadas_100m.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:areas_silvestres_protegidas"
```
