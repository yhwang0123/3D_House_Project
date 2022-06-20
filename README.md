# 3D House Project


plot a house in 3D with only a given address in Flanders

## Description

As Flanders of Belgium is divided into 43 zones, and the data of 43 zone is huge. I choose Province Antwerp as my target zones, with 12 zones in all. For any address in Province Antwerp, I can show the house in 3D model.

## Installation

The following libraries are used for this project:rioxarray
* requests
* json
* requests
* matplotlib
* os
*  pandas
*  plotly
*  os
* shapely
*  natsort
* fiona
* rasterio
*  time
* webbrowser
* mayavi
* Image

## Steps taken for the project


### Research

1. understand the DTM and DSM file
2. get to know the realtionship of CHM(The Canopy Height Model) with DTM and DSM
3. explore the libraries which can be used to deal with the GEO data
*  glob - to search all file with the same extension
* rasterio - read and write GEOTIFF format file
* rioarray - rasterio xarray extension (xarray - working with labelled multi-dimensional arrays)
* imageio - read and write image data
* plotly - plot 3D objects
* Mayavi - provide easy and interactive visualization of 3D data


### Data collecting
1.  DTM files for Flanders: http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dtm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DTM,%20raster,%201m
2.  DSM files for Flanders: https://www.geopunt.be/download?container=dhm-vlaanderen-ii-dsm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DSM,%20raster,%201m
3.  Data of each address in Flanders: https://api.basisregisters.vlaanderen.be


### Data Processing
Below diagram shows the process of my coding. It starts from input of an address, and output is the 3d plot of the house.   
![alt text](https://github.com/yhwang0123/3D_House_Project/blob/main/asset/workflow%20of%20coding.002.jpeg?raw=true)

## Example of 3D House

### Sint-Pietersvliet 7, 2000 Antwerpen
* 3d in plotly  

![alt text](https://github.com/yhwang0123/3D_House_Project/blob/main/asset/3d%20images/Sint-Pietersvliet%207.png?raw=true)

* 3d in Mayavia  
![alt text](https://github.com/yhwang0123/3D_House_Project/blob/main/asset/3d%20images/Sint-Pietersvliet%207%202000%20Antwerpen.png?raw=true)


### Kazernweg 35, 2950 Kapellen  

* 3d in plotly  
![alt text](https://github.com/yhwang0123/3D_House_Project/blob/main/asset/3d%20images/Kazernweg%2035.png?raw=true)
* 3d in Mayavia  
![alt text](https://github.com/yhwang0123/3D_House_Project/blob/main/asset/3d%20images/Kazernweg%2035%202950%20Kapellen.png?raw=true)

## Things to be improved
* overcome the ovelapping problem
