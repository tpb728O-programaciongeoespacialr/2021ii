```shell
# Aeródromos
$ ogr2ogr \
    -makevalid \
    aerodromos.geojson \
    WFS:"https://geos.snitcr.go.cr/be/IGN_200/wfs?version=1.1.0" "IGN_200:aerodromos_200k"

# Vías con geometrías simplificadas (500 m)
$ ogr2ogr \
    -simplify 500 \
    -makevalid \
    vias-simplificadas_500m.geojson \
    WFS:"http://geos.snitcr.go.cr/be/IGN_5/wfs" "IGN_5:vias_5000"  
```    
