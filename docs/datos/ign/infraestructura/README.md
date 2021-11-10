```shell
# Aeródromos
$ ogr2ogr \
    -makevalid \
    aerodromos.geojson \
    WFS:"https://geos.snitcr.go.cr/be/IGN_200/wfs?version=1.1.0" "IGN_200:aerodromos_200k"
```    
