---
title: "Leaflet_Map"
author: "Utkarsha Patil"
date: "February 25, 2019"
output:
  html_document: 
    fig_caption: yes
    keep_md: yes
    toc: yes
  pdf_document: default
  word_document: default
  md_document: default
---



## R Markdown with Leaflet 
Create a web page using R Markdown that features a map created with Leaflet.



```r
library(leaflet)
```

```
## Warning: package 'leaflet' was built under R version 3.5.2
```

```r
library(maps)

m <- leaflet() %>%
  addTiles() %>%  # Add default OpenStreetMap map tiles
  addMarkers(lng=-97.773, lat=30.269, popup="Popular park in Austin downtown")
m
```

<!--html_preserve--><div id="htmlwidget-cd49b673ba3dcceb7f9a" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-cd49b673ba3dcceb7f9a">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[30.269,-97.773,null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"Popular park in Austin downtown",null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[30.269,30.269],"lng":[-97.773,-97.773]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->
