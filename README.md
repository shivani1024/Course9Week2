# Course9Week2
Create a web page using R Markdown that features a map created with Leaflet.  Host your webpage on either GitHub Pages, RPubs, or NeoCities.  Your webpage must contain the date that you created the document, and it must contain a map created with Leaflet. We would love to see you show off your creativity!
---
title: "Birth place of R"
author: "Shivani Sawant"
date: "October 27, 2020"
output: 
  html_document: 
    keep_md: yes
---

## Plotting Map

The map below shows a view of birthplace of R. 

```{r Leaflet, echo=TRUE}
library(leaflet)
m <- leaflet()
m <- addTiles(m)
m <- addMarkers(m, lng=174.768, lat=-36.852, popup="The birthplace of R")
m
```
