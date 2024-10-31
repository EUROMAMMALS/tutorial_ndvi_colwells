---
title: "Tutorial to calculate Colwells metrics per grid cell"
output:
  html_document:
    css: html-md-01.css
    fig_caption: no
    number_sections: no
    toc: no
    toc_float: false
    collapsed: no
knit: (function(input, ...) {
    rmarkdown::render(
      input,
      output_file = 'index.html',
      envir = globalenv()
    )
  })
---

# Introduction 

Calculation of Colwells metrics (Predictibility, Constancy, Contingency) per grid cell using tiled raster datasets. In the example we use MODIS NDVI. Colwells metrics have been used within Euromammals by Mumme et al. ([2023](https://doi.org/10.1111/gcb.16769)).

# Directory Structure 

The repository contains the following files and directories:

```
. 
├── README.md
├── tutorial_ndvi_colwells.Rproj
├── code
│   ├── colwells.R
│   ├── colwells.Rmd
│   └── colwells.html
└── data
    └── 0_raw
        └── modis
            ├── MOD13A3_NDVI_2000_061.tif
            ├── MOD13A3_NDVI_2000_092.tif
            ├── MOD13A3_NDVI_2000_122.tif
            └── MOD13A3_NDVI_2000_153.tif
```


|           |   files/directories |  description          |
|-----------|---------------------|-----------------------|
| data      |      [0_raw/modis/](https://github.com/EUROMAMMALS/tutorial_ndvi_colwells/blob/main/data/0_raw/modis/)    | MODIS NDVI sample dataset  |
| code      |      [colwells.R](https://github.com/EUROMAMMALS/tutorial_ndvi_colwells/blob/main/code/colwells.R)    | R script              |            
|           |      [colwells.Rmd](https://github.com/EUROMAMMALS/tutorial_ndvi_colwells/blob/main/code/colwells.Rmd)   | R markdown version    |       
|           |      [colwells.html](https://github.com/EUROMAMMALS/tutorial_ndvi_colwells/blob/main/code/colwells.html)   | html version          |






