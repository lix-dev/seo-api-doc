# Serp API Documentation

#### Get Live Serps

Get live search results from google search engine (google.de)

**POST**

````javascript
/v1/serps/live
````

**PARAMETERS**

| Parameter | Value (example)                    | Description                                   |
| --------- | ---------------------------------- | --------------------------------------------- |
| keyword   | "pied piper"                       | (**required**) define a search term           |
| device    | "mobile" or "desktop"              | (**required**) define your device             |
| uule      | "w+CAIQICIOQmVybGluLEdlcm1hbnk"    | (**required**) define your location with uule |
| token     | "ndasocijiecwichwjecowcewcoijecwc" | (**required**) define your token              |

<br><br>

#### Get Geoloation uule code

Get a uule code from a location. We used google`s geotargets csv -> https://developers.google.com/adwords/api/docs/appendix/geotargeting

**POST**

````javascript
/v1/geotargets
````

**PARAMETERS**

| Parameter    | Value (example)                    | Description                      |
| ------------ | ---------------------------------- | -------------------------------- |
| term         | "berlin"                           | define a search term             |
| country_code | "DE"                               | define a country code            |
| target_type  | "City" or "Postal Code" or ...     | define the target type           |
| token        | "ndasocijiecwichwjecowcewcoijecwc" | (**required**) define your token |

