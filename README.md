# Wildfire Tracker Application

---

## Project Description

This project displays fires that still have the status "open" within the last 180 days. It is build using React, Google Maps React and NASA Open APIs.

## Project Background

In 2020 my family and I lost everything we had in a unexpected fast moving California Wildfire. Since then I have been attempting to create some sort of application that can better help determine the location burning fires.

---

## Running the Application Locally

Using your command line to navigate to the the projects folder, run the following in your terminal (intergrated or not)

##### Local React scripts

- To install the react project: npm install
- To run react (on port 3000): npm start

## Project `src` Tree

```
+--src
|   App.js
|   index.css
|   index.js
\   setupTests.js
    +--components
    |   Header.js
    |   Loader.js
    |   loading.gif
    |   LocationInfo.js
    |   LocationMarker.js
    \   Map.js
```

---

## About the API

**API Endpoint URL:** https://eonet.gsfc.nasa.gov/api/v2.1/events

**Optional Parameter used:** `?status=open&days=180`

### JSON Response Example

```
    {
      "id": "EONET_6195",
      "title": "Crockets Knob Fire",
      "description": "",
      "link": "https://eonet.gsfc.nasa.gov/api/v2.1/events/EONET_6195",
      "categories": [
        {
          "id": 8,
          "title": "Wildfires"
        }
      ],
      "sources": [
        {
          "id": "InciWeb",
          "url": "http://inciweb.nwcg.gov/incident/8355/"
        }
      ],
      "geometries": [
        {
          "date": "2022-08-22T03:00:00Z",
          "type": "Point",
          "coordinates": [
            -118.708,
            44.728000000000002
          ]
        }
      ]
    },

```
