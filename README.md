# Mexico Geographic Data

This repository contains a collection of JSON files with geographic and administrative data for Mexico.

## Contents

The data is organized into the following files:

* `states.json`: A list of the 32 states of Mexico, including their geographic coordinates (latitude and longitude).
* `counties.json`: A detailed list of all municipalities (counties) in Mexico, with their IDs, corresponding state names, and geographic coordinates.
* `settlements.json`: An extensive list of settlements (colonias, subdivisions, ranches, etc.) within the municipalities of Durango. Each entry includes a postal code, as well as the IDs and names of its state and county.

## Data Structure

Each JSON file is an array of objects. The structure for each dataset is as follows:

### `states.json`
* `id`: The unique identifier for the state.
* `name`: The official name of the state (e.g., "Durango").
* `lat`: The latitude of the state's geographic center.
* `lon`: The longitude of the state's geographic center.

### `counties.json`
* `id`: The unique identifier for the county/municipality.
* `stateId`: The ID of the state it belongs to.
* `stateName`: The name of the state it belongs to.
* `name`: The official name of the county/municipality (e.g., "Durango").
* `lat`: The latitude of the county's geographic center.
* `lon`: The longitude of the county's geographic center.

### `settlements.json`
* `id`: The unique identifier for the settlement.
* `name`: The name of the settlement (e.g., "Canatlán Centro").
* `lat`: (Optional) The latitude of the settlement.
* `lon`: (Optional) The longitude of the settlement.
* `postalCode`: The postal code of the settlement.
* `stateId`: The ID of the state it belongs to.
* `stateName`: The name of the state.
* `countyId`: The ID of the county it belongs to.
* `countyName`: The name of the county.

## How to Use

You can clone this repository to use these JSON files in your projects for data visualization, data analysis, or for populating databases.
