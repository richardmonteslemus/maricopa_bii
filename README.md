# Biodiversity Intactness Index change in Phoenix, AZ

**Author: [Richard Montes Lemus](https://richardmonteslemus.github.io/)**

# About

### File Structure
```
├── data
│   └── tl_2024_04_cousub
│       ├── tl_2024_04_cousub.cpg
│       ├── tl_2024_04_cousub.dbf
│       ├── tl_2024_04_cousub.prj
│       ├── tl_2024_04_cousub.shp
│       ├── tl_2024_04_cousub.shp.ea.iso.xml
│       ├── tl_2024_04_cousub.shp.iso.xml
│       └── tl_2024_04_cousub.shx
├── LICENSE
├── maricopa_bii.ipynb
└── README.md

```
### Purpose

Maricopa County contains the Phoenix metropolitan area and is the U.S. county with the most significant increase in developed land since 2001 (Levitt & Eng, 2021). This rapid urban sprawl has profound implications for biodiversity and the health of surrounding natural ecosystems.

This analysis will use Biodiversity Intactness Index (BII) to measure and visualize the impact of this urban expansion on ecosytems(Gassert et al., 2022). It will examine changes in BII in the Phoenix county subdivision area between 2017 and 2020, shedding light on how urban growth affects biodiversity over time.

### Highlights
* Load in Phoenix sub-divison data and explore 
* Access BII data and explore 
* Calculate difference in BII >= 0.75 between 2017 and 2020
* Create map representing areas with high biodiversity lost between 2017 and 2020 

### Data: 
**Biodiversity Intactness Index (BII) Time Series:** This BII time series can be obtained through the [Microsoft Planetary Computer STAC Catalog](https://planetarycomputer.microsoft.com/dataset/io-biodiversity). It contains a 2017 and 2020 raster covering the Phoenix subdivision. It is read in as `phx_bii`. 

**Phoenix Subdivision Shapefile:** This shapefile polygon can be obtained through [TIGER Shapefiles](https://www.census.gov/cgi-bin/geo/shapefiles/index.php). It contains Census County Subdivisions for Arizona. It is read in as `az_county`

| References |
|---------------------|
| Gassert, F., Mazzarello, J., & Hyde, S. (2022, August). Global 100m projections of biodiversity intactness for the years 2017-2020 [Technical whitepaper]. https://ai4edatasetspublicassets.blob.core.windows.net/assets/pdfs/io-biodiversity/Biodiversity_Intactness_whitepaper.pdf |
 Impact Observatory. (2022). 10m annual land use land cover (9-class) [Data set]. Microsoft Planetary Computer. https://planetarycomputer.microsoft.com/dataset/io-lulc-annual-v02 |
| Levitt, Z., & Eng, J. (2021, August). Where America's developed areas are growing: 'Way off into the horizon'. The Washington Post. https://www.washingtonpost.com/nation/interactive/2021/land-development-urban-growth-maps/ |
U.S. Census Bureau. (2023). TIGER/Line shapefiles: Arizona county subdivisions [Data set]. https://www2.census.gov/geo/tiger/TIGER2023/COUSUB/tl_2023_04_cousub.zip|
