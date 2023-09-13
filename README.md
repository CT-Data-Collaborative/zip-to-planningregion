# Connecticut ZIP to Planning Region Crosswalk

The zip-to-planningregion.xlsx file contains a crosswalk between CT zipcodes (technically 2020 ZCTAs, or zipcode tabulation areas, which are geographic approximations for zipcodes) and planning regions in CT.

There are 289 zipcodes and 9 planning regions in the state, and the crosswalk is a many-to-one relationship, meaning each zipcode points ("belongs") to only planning region.

Because some zipcodes cross planning region boundaries, this crosswalk is approximate.

# How it was generated
In QGIS, open zipcode boundaries, calculate their centroids, and perform nearest neighbor spatial join (NNJoin plugin) to assign the nearest planning region.

# Source datasets
Planning Region boundaries: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?layergroup=Counties%20%28and%20equivalent%29&year=2022

Zipcode (ZCTA) boundaries: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2022&layergroup=ZIP+Code+Tabulation+Areas

# License
Released under MIT license. Feel free to use for all sorts of projects. We will appreciate if you credited CTData Collaborative.
