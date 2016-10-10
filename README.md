Visualize my Hiking Trails 
=============

![GitHub version](https://img.shields.io/badge/version-1.0.0-green.svg)
[![HitCount](https://hitt.herokuapp.com/{ajpelu||org}/{hiking}.svg)](https://github.com/ajpelu/hiking)

This repo contains some code to explore my hiking trails and display them and some derived features into a map. 

The hiking trails, in [`.gpx`](http://www.topografix.com/gpx.asp) format are stored in the `/data/` folder. These files come from a GPS device. 

For each route a dashboard is created using [R Markdownd](http://rmarkdown.rstudio.com/) and [flexdashboard](http://rmarkdown.rstudio.com/flexdashboard/index.html). In the `/analysis/` folder there are two files for each trail: a `.Rmd` file with the code, and a `.html` file (the rendered dashboard). 



# Routes 
* [Climb Mulhacen (Sierra Nevada, Spain) - 2016-August](https://rawgit.com/ajpelu/hiking/master/analysis/2016_mulhacen.html) 

* [Tajos de la Virgen - Elorrieta (Sierra Nevada, Spain) - 2016-August](https://rawgit.com/ajpelu/hiking/master/analysis/2016_elorrieta.html)

* [Barranco de las Ánimas, Collado del Diablo (Sierra Nevada, Spain) - 2016-October](https://rawgit.com/ajpelu/hiking/master/analysis/2016_sn_barranco_Animas.html)

* [Barranco de las Yegueros (Tajos de Breca), Bérchules (Sierra Nevada, Spain) - 2016-October](https://rawgit.com/ajpelu/hiking/master/analysis/2016_sn_barranco_YeguerosBerchules.html)


# More info:
* [@ajpelu](https://twitter.com/ajpelu)
* [ajperezluque.com](http://ajperezluque.com)

# Version 
![GitHub version](https://img.shields.io/badge/version-1.0.0-green.svg)

# License 
This repository is licenced as Creative Commons Attribution 4.0 ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)). You can find more info [here](/LICENSE). Anyone can use the content of the repository citing as followging:

* Pérez-Luque AJ (2016). Visualize my Hiking Trails. ![](https://img.shields.io/badge/version-1.0.0-green.svg). [https://github.com/ajpelu/hiking](https://github.com/ajpelu/hiking) 

# Sources
This idea is inspired on several sources. In the following list you can find them and the sources used to build this site. 

* Maarte Hermans's [post](http://mhermans.net/hiking-gpx-r-leaflet.html)
* Notes on Using WMS in Leaflet (P. Soriano) [post](http://sigdeletras.github.io/Leaflet.Spain.WMS/examples/)
* Flexdashboard documentation [page](http://rmarkdown.rstudio.com/flexdashboard/index.html)
* [BikeHike](http://bikehike.co.uk/index.php) 
* Dan Goldin [post](http://dangoldin.com/2014/02/05/visualizing-gps-data-in-r/) 
* [Links about routes](/man/Usefuls_Routes_Links.md)
 