# morocco-region-city-coordinates
A list of Moroccan cities with their respective coordinates

# Install
`npm i morocco-region-city-coordinates`

# Docs

Country.getCountryByCode(countryCode)
---------------

It accepts Morocco's `CountryCode` eg: `'MA'` and   returns *Country Details*

type: **json | ICountry**

```js
{
    "name": "Morocco",
    "isoCode": "MA",
    "flag": "🇲🇦",
    "phonecode": "212",
    "currency": "MAD",
    "latitude": "32.00000000",
    "longitude": "-5.00000000",
    "timezones": [
        {
            "zoneName": "Africa/Casablanca",
            "gmtOffset": 3600,
            "gmtOffsetName": "UTC+01:00",
            "abbreviation": "WEST",
            "tzName": "Western European Summer Time"
        }
    ]
}
```

State.getStateByCodeAndCountry(stateCode, countryCode)
---------------

It accepts a valid `StateCode` eg: `'01'` `CountryCode` eg: `'MA'` and   returns *State Details*

type: **json | ICountry**

```js
{
    "name": "Tanger-Tétouan-Al Hoceïma",
    "isoCode": "01",
    "countryCode": "MA",
    "latitude": "35.26295580",
    "longitude": "-5.56172790"
}
```

State.getStatesOfCountry(countryCode)
---------------

It accepts Morocco's `CountryCode` and returns *all States* as Array of JSON

type: **array of json | IState**

```js
[
	{
    "name": "Tanger-Tétouan-Al Hoceïma",
    "isoCode": "01",
    "countryCode": "MA",
    "latitude": "35.26295580",
    "longitude": "-5.56172790"
    }
]

```
City.getCitiesOfState(countryCode, stateCode)
---------------

It accepts Morocco's `CountryCode` and a valid `StateCode` and returns *all Cities* as Array of JSON

type: **array of json | ICity**

```js
[
	{
        "name": "Tanger",
        "countryCode": "MA",
        "stateCode": "01",
        "latitude": "35.7595",
        "longitude": "-5.8340"
    }
]

```

City.getCitiesOfCountry(countryCode)
---------------

It accepts Morocco's `CountryCode` and returns *all Cities* as Array of JSON

type: **array of json | ICity**

```js
[
	{
        "name": "Tanger",
        "countryCode": "MA",
        "stateCode": "01",
        "latitude": "35.7595",
        "longitude": "-5.8340"
    }
]

```

Country.getAllCountries
---------------
It returns **all Countries** (Morocco Only)

type: **array of json | ICountry**

```js
[
	{
        "name": "Morocco",
        "isoCode": "MA",
        "flag": "🇲🇦",
        "phonecode": "212",
        "currency": "MAD",
        "latitude": "32.00000000",
        "longitude": "-5.00000000",
        "timezones": [
            {
                "zoneName": "Africa/Casablanca",
                "gmtOffset": 3600,
                "gmtOffsetName": "UTC+01:00",
                "abbreviation": "WEST",
                "tzName": "Western European Summer Time"
            }
    ]
    }
]
```

State.getAllStates
---------------
It returns **all States**

type: **array of json | IState**

```js
[
	{
    "name": "Tanger-Tétouan-Al Hoceïma",
    "isoCode": "01",
    "countryCode": "MA",
    "latitude": "35.26295580",
    "longitude": "-5.56172790"
    }
]
```

City.getAllCities
---------------
It returns **all Cities**

type: **array of json | ICity**

```js
[
	{
        "name": "Tanger",
        "countryCode": "MA",
        "stateCode": "01",
        "latitude": "35.7595",
        "longitude": "-5.8340"
    }
]
```