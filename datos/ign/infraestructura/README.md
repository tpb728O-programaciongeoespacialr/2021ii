```shell
# Aeródromos
$ ogr2ogr \
    -makevalid \
    aerodromos.geojson \
    WFS:"https://geos.snitcr.go.cr/be/IGN_200/wfs?version=1.1.0" "IGN_200:aerodromos_200k"

# Red vial
$ ogr2ogr \
    -makevalid \
    redvial.geojson \
    WFS:"https://geos.snitcr.go.cr/be/IGN_200/wfs?version=1.1.0" "IGN_200:redvial_200k"  

# Red vial con geometrías simplificadas (100 m)
$ ogr2ogr \
    -simplify 100 \
    -makevalid \
    redvial-simplificadas_100m.geojson \
    WFS:"https://geos.snitcr.go.cr/be/IGN_200/wfs?version=1.1.0" "IGN_200:redvial_200k" 
  
# Red vial con geometrías simplificadas (500 m)
$ ogr2ogr \
    -simplify 500 \
    -makevalid \
    redvial-simplificadas_500m.geojson \
    WFS:"https://geos.snitcr.go.cr/be/IGN_200/wfs?version=1.1.0" "IGN_200:redvial_200k"    
```    
