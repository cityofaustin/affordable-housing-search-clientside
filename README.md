# AffordableHousingSearchToolFinal

The AffordableHousingSearchToolFinal is a mobile responsive web application created as part of a Code for America Community Fellowship in Austin TX. It can be used on a desktop browser but is primarily meant for mobile users. It allows users to search for Affordable Housing inventory by connecting to Austin's AffordableHousingDataHub. An instance of this application was deployed for Austin TX so that residents could have one place to access the entirety of Austin's affordable housing inventory, and also filter by critiera that fit their specific needs.

### Technologies

This code is a modification of the repo found here: https://github.com/cityofaustin/AffordableHousingSearchToolFinal-fork
This code is client side only. It uses javascript / JQuery / css. It uses Leaflet's javascript library for interactive maps, with a dependency on Mapbox's API. A Mapbox service account will be needed to utilize this Mapbox mapping layer that is built into the application. Any API can be used to retrieving housing data, but the one configured by default by this project is Austin's AffordableHousingDataHub.

### Installation

1. **Create an additional file:** `mapbox_public_key.js`. This file should include a variable called `mapbox_public_key`, which should be set to the public key (string) that you get from mapbox. A public key from mapbox is required in order to access the mapping layer utlized by this application. In order to generate one, you will need to create a mapbox account for local development. The file `mapbox_public_key.js` is ignored by git by default. See here for more information about requesting an access token: https://www.mapbox.com/account/access-tokens/.
2. **Create an additional file:** `data_hub_api_endpoint.js`. This file should include a variable called `data_hub_api_endpoint`, which should be set to the `get_all_data.json` endpoint from your local development environment (i.e., https://localhost:3000/get_all_data.json, the online development portal (i.e., https://dev-portal.atxaffordablehousing.net/get_all_data.json), the staging portal (i.e., https://stage-portal.atxaffordablehousing.net/get_all_data.json, or the production portal (i.e., https://portal.atxaffordablehousing.net/get_all_data.json). The file `data_hub_api_endpoint.js` is ignored by git by default.
3. **Launch the Search Tool**: Open `index.html`
