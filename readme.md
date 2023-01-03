# Notes on the

### Obtaining the Data 

- Listings for **sale** properties in County Dublin are scraped from Daft.ie, using Playwright and BeautifulSoup.

### Obtaining the Geometry 

- The latitude and longitude coordinates for each listing were obtained using the Google Maps Geocoding API: 
    https://developers.google.com/maps/documentation/geocoding/overview

### Joining the basemap and the data 

- Basemap downloaded from here: 
    https://autoaddress.com/en-ie/support/developer-centre/resources/routing-key-boundaries 
- Basemap and data joined to obtain statistics **grouped by Eircode routing district**
- Done in QGIS using the Vector -> Intersection tool 
