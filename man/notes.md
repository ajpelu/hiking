# Sources

* http://mhermans.net/hiking-gpx-r-leaflet.html 
* http://ionicons.com/
* FontAwesome 


# Issues 
* Add plotkml 3d map. See http://gsif.isric.org/doku.php/wiki:tutorial_plotkml 


# Some old notes 


Read Sierra Nevada limits
enp <- rgdal::readOGR(dsn='/Users/ajpeluLap/Downloads/EENNPP/InfGeografica/InfVectorial/Shapes/ED50_30', 
                      layer = 'EENNPP', verbose = FALSE)

sn <- subset(enp, NOMBRE == 'SIERRA NEVADA' & FIGURA == 'Espacio Natural')

# Reproject to lat / lon W
# reproject naamp to lat/lon WGS84 ("geographic projection")
sn_ll <- spTransform(sn, CRS("+proj=longlat"))


ib <- leaflet() %>% 
  setView(lng=-3.69, lat=40, zoom=5) %>%
  addProviderTiles('Esri.WorldShadedRelief')
  #addProviderTiles('Stamen.TerrainBackground')

print(ib)
    

mymap <- leaflet() %>% 
  setView(-3, 37, zoom=8) %>% 
 addProviderTiles('Esri.WorldShadedRelief') %>%
#   # addWMSTiles('http://www.juntadeandalucia.es/medioambiente/mapwms/REDIAM_mapa_guia_pn_sierra_nevada_2007?',
#               layers = '1',
#               options = WMSTileOptions(format = "image/png", transparent = TRUE),
              # attribution = "") %>%
  addPolygons(sn_ll, stroke = FALSE, fillOpacity = 0.5, smoothFactor = 0.5)
    
    


states <- readOGR('/Users/ajpeluLap/Downloads/EENNPP/InfGeografica/InfVectorial/Shapes/ED50_30/EENNPP.shp', 
                  layer='EENNPP', verbose = FALSE)

sn <- subset(states, FIGURA == 'Espacio Natural', NOMBRE == 'SIERRA NEVADA')


