# Property Prices in Dublin

This project scrapes property listing prices and aggregates them on a map. 

View the map [here](https://kellywaldro.github.io/dublin_properties/)

### Obtaining the Data 

- Listings for **sale** properties in County Dublin are scraped from Daft.ie, using Playwright and BeautifulSoup in `Scrape.ipynb`

### Obtaining the Geometry 

- The latitude and longitude coordinates for each listing were obtained using the [Google Maps Geocoding API](   https://developers.google.com/maps/documentation/geocoding/overview) in `Cleaning.ipynb`

### Joining the basemap and the data 

- Basemap downloaded from [here](https://autoaddress.com/en-ie/support/developer-centre/resources/routing-key-boundaries)
- Basemap and data joined to obtain statistics **grouped by Eircode routing district** (more about Eircodes [here](https://www.eircode.ie/what-is-eircode)
- Done in QGIS using the Vector -> Intersection tool 

### Published on webpage 

- Data joined to geojson and published using Mapbox GL JS in `df_to_maps.ipynb`



