# Cars

## Create a Car

```shell
curl "https://staging.financial.leasedesk.nl/api/v1/car/create
    -X POST
    -H "Authorization: Bearer <your_access_token>"
    -H "Content-Type: application/json"
    -H "Accept: application/json"
    --data {
       "advertiser_id": 1,
       "license_plate_number": "PD839Z",
       "chassis_number": null,
       "brand": "Opel",
       "type": "Corsa",
       "serie": "1.4-16V DESIGN EDITION 5-Drs Airco LM16",
       "description": "Modelreeks, informatie, etc",
       "body_type": "HB",
       "fuel_type": "B",
       "fuel_consumption_city": "16",
       "fuel_consumption_highway": "23",
       "fuel_consumption_combined": "20",
       "transmission_type": "H",
       "transmission_amount": 5,
       "color": "geel",
       "color_brand": null,
       "mileage": 59638,
       "mileage_type": "KM",
       "nap_valid": false,
       "engine_cylinders": 4,
       "engine_capacity": 1600,
       "engine_power": 74,
       "engine_power_type": "KW",
       "engine_top_speed": 180,
       "engine_top_speed_type": "KM",
       "emission_co2": 120,
       "load_capacity": 577,
       "doors": 5,
       "seats": 5,
       "keys_amount": 2,
       "weight": 1063,
       "construction_date": "2014-01-01",
       "apk_due_date": "2018-11-26",
       "price_excl_vat": 10450,
       "price_incl_vat": 10450,
       "price_delivery": 0,
       "price_bpm": 1051,
       "tax_benefit": 25,
       "tax_road_min": "117.00",
       "tax_road_max": "130.00",
       "accessories": [
           "3e remlicht",
           "Airbag(s) hoofd en side",
           "Airbag bestuurder en passagier",
           "Airco",
           "Alarm klasse 1(startblokkering)",
           "Anti blokkeer systeem",
           "AUX-ingang",
           "Bestuurdersstoel in hoogte verstelbaar",
           "Boordcomputer",
           "Buitenspiegels elektrisch verstelbaar",
           "Centrale deurvergrendeling met afstandsbediening",
           "Cruise control",
           "Electronic stability program",
           "Elektrische ramen voor",
           "Extra getint glas",
           "Hoofdsteunen achter",
           "Isofix",
           "Lederen stuurwiel",
           "Lichtmetalen velgen 16\"",
           "Mistlampen voor",
           "Multimedia-voorbereiding",
           "Navigatie systeem af fabriek",
           "Radio-cd/mp3 speler",
           "Ruitenwisser achter",
           "Stuur verstelbaar",
           "USB-poort"
       ],
       "videos": [
           {
               "type": "YT",
               "url": "https://www.youtube.com/v/4160NvEhThA"
           }
       ],
       "images": [
        "http://google.com/image.jpg",
        "http://google.com/image2.jpg",
        "http://google.com/image3.jpg"
       ]
   }
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 1,
        "advertiser": {
            "id": 1,
            "advertiser_id": "test_124",
            "name": "Autobedrijf Janssen",
            "street": "Stationstraat",
            "number": "10",
            "number_extra": "a",
            "zipcode": "1234AB",
            "city": "Maastricht",
            "country": "Nederland",
            "phone": "+31 40 123 45 67",
            "email": "info@autobedrijfjassen.nl",
            "web": "http://autobedrijfjanssen.nl",
            "created_at": "20-02-2018 09:47:22",
            "updated_at": "20-02-2018 09:47:22"
        },
        "license_plate_number": "PD839Z",
        "chassis_number": null,
        "brand": "Opel",
        "type": "Corsa",
        "serie": "1.4-16V DESIGN EDITION 5-Drs Airco LM16",
        "description": "Modelreeks, informatie, etc",
        "body_type": "HB",
        "fuel_type": "B",
        "fuel_consumption_city": 16,
        "fuel_consumption_highway": 23,
        "fuel_consumption_combined": 20,
        "transmission_type": "H",
        "transmission_amount": 5,
        "color": "geel",
        "color_brand": null,
        "mileage": 59638,
        "mileage_type": "KM",
        "nap_valid": false,
        "engine_cylinders": 4,
        "engine_capacity": 1600,
        "engine_power": 74,
        "engine_power_type": "KW",
        "engine_top_speed": 180,
        "engine_top_speed_type": "KM",
        "emission_co2": 120,
        "load_capacity": 577,
        "doors": 5,
        "seats": 5,
        "keys_amount": 2,
        "weight": 1063,
        "construction_date": "2014-01-01 00:00:00",
        "apk_due_date": "2018-11-26 00:00:00",
        "price_excl_vat": "10450.00",
        "price_incl_vat": "10450.00",
        "price_delivery": "0.00",
        "price_bpm": "1051.00",
        "tax_benefit": 25,
        "tax_road_min": "117.00",
        "tax_road_max": "130.00",
        "accessories": [
            "3e remlicht",
            "Airbag(s) hoofd en side",
            "Airbag bestuurder en passagier",
            "Airco",
            "Alarm klasse 1(startblokkering)",
            "Anti blokkeer systeem",
            "AUX-ingang",
            "Bestuurdersstoel in hoogte verstelbaar",
            "Boordcomputer",
            "Buitenspiegels elektrisch verstelbaar",
            "Centrale deurvergrendeling met afstandsbediening",
            "Cruise control",
            "Electronic stability program",
            "Elektrische ramen voor",
            "Extra getint glas",
            "Hoofdsteunen achter",
            "Isofix",
            "Lederen stuurwiel",
            "Lichtmetalen velgen 16\"",
            "Mistlampen voor",
            "Multimedia-voorbereiding",
            "Navigatie systeem af fabriek",
            "Radio-cd/mp3 speler",
            "Ruitenwisser achter",
            "Stuur verstelbaar",
            "USB-poort"
        ],
        "videos": [
            {
                "type": "YT",
                "url": "https://www.youtube.com/v/RICBjWLwupw"
            }
        ],
        "images": [
            "http://google.com/image.jpg",
            "http://google.com/image2.jpg",
            "http://google.com/image3.jpg"
        ],
        "created_at": "20-02-2018 09:47:39",
        "updated_at": "20-02-2018 09:50:27",
        "url": "http://staging.financial.leasedesk.nl/aanbod/1"
    }
}
```

This endpoint creates a new Car.

<aside class="warning">Make sure you send the json payload as raw body data to the endpoint. Also remember that the advertiser ID should be equal to the ID returned by your call when creating an Advertiser!</aside>

### HTTP Request

`POST https://staging.financial.leasedesk.nl/api/v1/car/create`

### Raw Body Parameters (JSON)

Parameter | Description | Required | Validation
--------- | ----------- | -------- | ----------
advertiser_id | The ID a given by the Advertiser endpoint | Yes | *existing ID as returned by Advertiser endpoint*
license_plate_number | The license plate number | Yes | 
brand | The brand name | Yes | 
type | The type name | Yes | 
serie | The series description | Yes | 
description | Full car description | No | 
color | The color of the car | Yes | 
color_brand | The factory name of the color | No | 
fuel_type | The fuel type (see below) | Yes | *in: B,D,E,EB,ED,LPG,O*
fuel_consumption_city | Fuel consumption in the city in KM per Liter | No | *numeric*
fuel_consumption_highway | Fuel consumption on the highway in KM per Liter | No | *numeric*
fuel_consumption_combined | Fuel consumption average in KM per Liter | No | *numeric*
transmission_type | Transmission type (see below) | Yes | *in: H,A,O*
transmission_amount | The amount of gears | No | *integer*
body_type | The body type (see below) | Yes | *in: HB,CB,CP,SUV,SD,SW,MPV,CC,O*
construction_date | The construction date | Yes | *date:Y-m-d*
mileage | The mileage amount | Yes | *integer*
mileage_type | The mileage type (see below) | Yes | *in: KM,M*
doors | The number of doors | No | *integer*
engine_cylinders | The number of cylinders | No | *integer*
engine_capacity | Engine capacity in cc | No | *integer*
engine_power | The power of the engine | Yes | *integer*
engine_power_type | The power type (see below) | Yes | *in: PK,KW*
engine_top_speed | The top speed of the vehicle | No | *integer*
engine_top_speed_type | The speed type (see below) | No | *in: KM,M*
apk_due_date | Due date for the yearly check-up | No | *date:Y-m-d*
nap_valid | Does the car have a valid NAP? | No | *boolean*
price_excl_vat | Pricing excl VAT | Yes | *numeric*
price_incl_vat | Pricing incl VAT | Yes | *numeric*
price_delivery | Delivery costs | Yes | *numeric*
price_bpm | The BPM amount | No | *numeric*
chassis_number | The chassisnumber | No |
keys_amount | Amount of available keys | No | *integer*
emission_co2 | The co2 emission in g/km | No | *integer*
seats | The amount of seats | No | *integer*
load_capacity | The load capacity in Liter | No | *integer*
weight | The weight in kilogram | Yes | *integer*
tax_benefit | Tax benefit class in percent | Yes | *numeric*
road_tax_min | Minimum amount of road tax | Yes | *numeric*
road_tax_max | Maximum amount of road tax | Yes | *numeric*
images | Array of images (see below) | Yes | *array*
videos | Array of videos (see below) | No | *array*
accessories | Array of accessores (see below) | No | *array*

## Update a Car

```shell
curl "https://staging.financial.leasedesk.nl/api/v1/car/<ID>
    -X PUT
    -H "Authorization: Bearer <your_access_token>"
    -H "Content-Type: application/json"
    -H "Accept: application/json"
    --data {
       "advertiser_id": 1,
       "license_plate_number": "AABB11",
       "chassis_number": null,
       "brand": "Opel",
       "type": "Corsa",
       "serie": "1.4-16V DESIGN EDITION 5-Drs Airco LM16",
       "description": "Modelreeks, informatie, etc",
       "body_type": "HB",
       "fuel_type": "B",
       "fuel_consumption_city": "16",
       "fuel_consumption_highway": "23",
       "fuel_consumption_combined": "20",
       "transmission_type": "H",
       "transmission_amount": 5,
       "color": "geel",
       "color_brand": null,
       "mileage": 59638,
       "mileage_type": "KM",
       "nap_valid": false,
       "engine_cylinders": 4,
       "engine_capacity": 1600,
       "engine_power": 74,
       "engine_power_type": "KW",
       "engine_top_speed": 180,
       "engine_top_speed_type": "KM",
       "emission_co2": 120,
       "load_capacity": 577,
       "doors": 5,
       "seats": 5,
       "keys_amount": 2,
       "weight": 1063,
       "construction_date": "2014-01-01",
       "apk_due_date": "2018-11-26",
       "price_excl_vat": 10450,
       "price_incl_vat": 10450,
       "price_delivery": 0,
       "price_bpm": 1051,
       "tax_benefit": 25,
       "tax_road_min": "117.00",
       "tax_road_max": "130.00",
       "accessories": [
           "3e remlicht",
           "Airbag(s) hoofd en side",
           "Airbag bestuurder en passagier",
           "Airco",
           "Alarm klasse 1(startblokkering)",
           "Anti blokkeer systeem",
           "AUX-ingang",
           "Bestuurdersstoel in hoogte verstelbaar",
           "Boordcomputer",
           "Buitenspiegels elektrisch verstelbaar",
           "Centrale deurvergrendeling met afstandsbediening",
           "Cruise control",
           "Electronic stability program",
           "Elektrische ramen voor",
           "Extra getint glas",
           "Hoofdsteunen achter",
           "Isofix",
           "Lederen stuurwiel",
           "Lichtmetalen velgen 16\"",
           "Mistlampen voor",
           "Multimedia-voorbereiding",
           "Navigatie systeem af fabriek",
           "Radio-cd/mp3 speler",
           "Ruitenwisser achter",
           "Stuur verstelbaar",
           "USB-poort"
       ],
       "videos": [
           {
               "type": "YT",
               "url": "https://www.youtube.com/v/4160NvEhThA"
           }
       ],
       "images": [
        "http://google.com/image.jpg",
        "http://google.com/image2.jpg",
        "http://google.com/image3.jpg"
       ]
   }
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 1,
        "advertiser": {
            "id": 1,
            "name": "Autobedrijf Janssen",
            "street": "Stationstraat",
            "number": "10",
            "number_extra": "a",
            "zipcode": "1234AB",
            "city": "Maastricht",
            "country": "Nederland",
            "phone": "+31 40 123 45 67",
            "email": "info@autobedrijfjassen.nl",
            "web": "http://autobedrijfjanssen.nl",
            "created_at": "20-02-2018 09:47:22",
            "updated_at": "20-02-2018 09:47:22"
        },
        "license_plate_number": "AABB11",
        "chassis_number": null,
        "brand": "Opel",
        "type": "Corsa",
        "serie": "1.4-16V DESIGN EDITION 5-Drs Airco LM16",
        "description": "Modelreeks, informatie, etc",
        "body_type": "HB",
        "fuel_type": "B",
        "fuel_consumption_city": 16,
        "fuel_consumption_highway": 23,
        "fuel_consumption_combined": 20,
        "transmission_type": "H",
        "transmission_amount": 5,
        "color": "geel",
        "color_brand": null,
        "mileage": 59638,
        "mileage_type": "KM",
        "nap_valid": false,
        "engine_cylinders": 4,
        "engine_capacity": 1600,
        "engine_power": 74,
        "engine_power_type": "KW",
        "engine_top_speed": 180,
        "engine_top_speed_type": "KM",
        "emission_co2": 120,
        "load_capacity": 577,
        "doors": 5,
        "seats": 5,
        "keys_amount": 2,
        "weight": 1063,
        "construction_date": "2014-01-01 00:00:00",
        "apk_due_date": "2018-11-26 00:00:00",
        "price_excl_vat": "10450.00",
        "price_incl_vat": "10450.00",
        "price_delivery": "0.00",
        "price_bpm": "1051.00",
        "tax_benefit": 25,
        "tax_road_min": "117.00",
        "tax_road_max": "130.00",
        "accessories": [
            "3e remlicht",
            "Airbag(s) hoofd en side",
            "Airbag bestuurder en passagier",
            "Airco",
            "Alarm klasse 1(startblokkering)",
            "Anti blokkeer systeem",
            "AUX-ingang",
            "Bestuurdersstoel in hoogte verstelbaar",
            "Boordcomputer",
            "Buitenspiegels elektrisch verstelbaar",
            "Centrale deurvergrendeling met afstandsbediening",
            "Cruise control",
            "Electronic stability program",
            "Elektrische ramen voor",
            "Extra getint glas",
            "Hoofdsteunen achter",
            "Isofix",
            "Lederen stuurwiel",
            "Lichtmetalen velgen 16\"",
            "Mistlampen voor",
            "Multimedia-voorbereiding",
            "Navigatie systeem af fabriek",
            "Radio-cd/mp3 speler",
            "Ruitenwisser achter",
            "Stuur verstelbaar",
            "USB-poort"
        ],
        "videos": [
            {
                "type": "YT",
                "url": "https://www.youtube.com/v/RICBjWLwupw"
            }
        ],
        "images": [
            "http://google.com/image.jpg",
            "http://google.com/image2.jpg",
            "http://google.com/image3.jpg"
        ],
        "created_at": "20-02-2018 09:47:39",
        "updated_at": "20-02-2018 09:50:27",
        "url": "http://staging.financial.leasedesk.nl/aanbod/1"
    }
}
```

This endpoint updates an existing Car.

<aside class="warning">Make sure you send the json payload as raw body data to the endpoint.</aside>

### HTTP Request

`PUT https://staging.financial.leasedesk.nl/api/v1/car/<ID>`

### Raw Body Parameters (JSON)

Parameter | Description | Required | Validation
--------- | ----------- | -------- | ----------
advertiser_id | The ID a given by the Advertiser endpoint | Yes | *existing ID as returned by Advertiser endpoint*
license_plate_number | The license plate number | Yes | 
brand | The brand name | Yes | 
type | The type name | Yes | 
serie | The series description | Yes | 
description | Full car description | No | 
color | The color of the car | Yes | 
color_brand | The factory name of the color | No | 
fuel_type | The fuel type (see below) | Yes | *in: B,D,E,EB,ED,LPG,O*
fuel_consumption_city | Fuel consumption in the city in KM per Liter | No | *numeric*
fuel_consumption_highway | Fuel consumption on the highway in KM per Liter | No | *numeric*
fuel_consumption_combined | Fuel consumption average in KM per Liter | No | *numeric*
transmission_type | Transmission type (see below) | Yes | *in: H,A,O*
transmission_amount | The amount of gears | No | *integer*
body_type | The body type (see below) | Yes | *in: HB,CB,CP,SUV,SD,SW,MPV,CC,O*
construction_date | The construction date | Yes | *date:Y-m-d*
mileage | The mileage amount | Yes | *integer*
mileage_type | The mileage type (see below) | Yes | *in: KM,M*
doors | The number of doors | No | *integer*
engine_cylinders | The number of cylinders | No | *integer*
engine_capacity | Engine capacity in cc | No | *integer*
engine_power | The power of the engine | Yes | *integer*
engine_power_type | The power type (see below) | Yes | *in: PK,KW*
engine_top_speed | The top speed of the vehicle | No | *integer*
engine_top_speed_type | The speed type (see below) | No | *in: KM,M*
apk_due_date | Due date for the yearly check-up | No | *date:Y-m-d*
nap_valid | Does the car have a valid NAP? | No | *boolean*
price_excl_vat | Pricing excl VAT | Yes | *numeric*
price_incl_vat | Pricing incl VAT | Yes | *numeric*
price_delivery | Delivery costs | Yes | *numeric*
price_bpm | The BPM amount | No | *numeric*
chassis_number | The chassisnumber | No |
keys_amount | Amount of available keys | No | *integer*
emission_co2 | The co2 emission in g/km | No | *integer*
seats | The amount of seats | No | *integer*
load_capacity | The load capacity in Liter | No | *integer*
weight | The weight in kilogram | Yes | *integer*
tax_benefit | Tax benefit class in percent | No | *numeric*
road_tax_min | Minimum amount of road tax | Yes | *numeric*
road_tax_max | Maximum amount of road tax | Yes | *numeric*
images | Array of images (see below) | Yes | *array*
videos | Array of videos (see below) | No | *array*
accessories | Array of accessores (see below) | No | *array*

## Get All Cars

```shell
curl "https://staging.financial.leasedesk.nl/api/v1/car"
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            /*full car response*/
        },
        {
            /*full car2 response*/
        }
    ]
}
```

This endpoint retrieves all Cars created by the currently authenticated client.

### HTTP Request

`GET https://staging.financial.leasedesk.nl/api/v1/car`

### Query Parameters

None

<aside class="success">
Remember — don't forget to authenticate!
</aside>

## Get a Specific Car

```shell
curl "https://staging.financial.leasedesk.nl/api/v1/car/1"
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": 1,
        "advertiser": {
            "id": 1,
            "name": "Autobedrijf Janssen",
            "street": "Stationstraat",
            "number": "10",
            "number_extra": "a",
            "zipcode": "1234AB",
            "city": "Maastricht",
            "country": "Nederland",
            "phone": "+31 40 123 45 67",
            "email": "info@autobedrijfjassen.nl",
            "web": "http://autobedrijfjanssen.nl",
            "created_at": "20-02-2018 09:47:22",
            "updated_at": "20-02-2018 09:47:22"
        },
        "license_plate_number": "PD839Z",
        "chassis_number": null,
        "brand": "Opel",
        "type": "Corsa",
        "serie": "1.4-16V DESIGN EDITION 5-Drs Airco LM16",
        "description": "Modelreeks, informatie, etc",
        "body_type": "HB",
        "fuel_type": "B",
        "fuel_consumption_city": 16,
        "fuel_consumption_highway": 23,
        "fuel_consumption_combined": 20,
        "transmission_type": "H",
        "transmission_amount": 5,
        "color": "geel",
        "color_brand": null,
        "mileage": 59638,
        "mileage_type": "KM",
        "nap_valid": false,
        "engine_cylinders": 4,
        "engine_capacity": 1600,
        "engine_power": 74,
        "engine_power_type": "KW",
        "engine_top_speed": 180,
        "engine_top_speed_type": "KM",
        "emission_co2": 120,
        "load_capacity": 577,
        "doors": 5,
        "seats": 5,
        "keys_amount": 2,
        "weight": 1063,
        "construction_date": "2014-01-01 00:00:00",
        "apk_due_date": "2018-11-26 00:00:00",
        "price_excl_vat": "10450.00",
        "price_incl_vat": "10450.00",
        "price_delivery": "0.00",
        "price_bpm": "1051.00",
        "tax_benefit": 25,
        "tax_road_min": "117.00",
        "tax_road_max": "130.00",
        "accessories": [
            "3e remlicht",
            "Airbag(s) hoofd en side",
            "Airbag bestuurder en passagier",
            "Airco",
            "Alarm klasse 1(startblokkering)",
            "Anti blokkeer systeem",
            "AUX-ingang",
            "Bestuurdersstoel in hoogte verstelbaar",
            "Boordcomputer",
            "Buitenspiegels elektrisch verstelbaar",
            "Centrale deurvergrendeling met afstandsbediening",
            "Cruise control",
            "Electronic stability program",
            "Elektrische ramen voor",
            "Extra getint glas",
            "Hoofdsteunen achter",
            "Isofix",
            "Lederen stuurwiel",
            "Lichtmetalen velgen 16\"",
            "Mistlampen voor",
            "Multimedia-voorbereiding",
            "Navigatie systeem af fabriek",
            "Radio-cd/mp3 speler",
            "Ruitenwisser achter",
            "Stuur verstelbaar",
            "USB-poort"
        ],
        "videos": [
            {
                "type": "YT",
                "url": "https://www.youtube.com/v/RICBjWLwupw"
            }
        ],
        "images": [
            "http://google.com/image.jpg",
            "http://google.com/image2.jpg",
            "http://google.com/image3.jpg"
        ],
        "created_at": "20-02-2018 09:47:39",
        "updated_at": "20-02-2018 09:50:27",
        "url": "http://staging.financial.leasedesk.nl/aanbod/1"
    }
}
```

This endpoint retrieves a specific Car.

<aside class="warning">If you try to get an advertiser that wasn't added by your client a HTTP error will be returned.</aside>

### HTTP Request

`GET https://staging.financial.leasedesk.nl/api/v1/car/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the Car to retrieve

## Delete a Specific Car

```shell
curl "https://staging.financial.leasedesk.nl/api/v1/car/1"
  -X DELETE
  -H "Authorization: Bearer <your_access_token>"
```

> The above command returns JSON structured like this:

```json
[]
```

This endpoint deletes a specific Car.

<aside class="warning">The JSON response will be empty, when the Car is deleted succesfully a HTTP 200 OK response will be returned.</aside>

### HTTP Request

`DELETE https://staging.financial.leasedesk.nl/api/v1/car/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the Car to delete

## Field type description

Some fields have abbreviated values, below you can find what each value means.

### fuel_type

Value | Description
----- | -----------
B | Benzine
D | Diesel
E | Elektrisch
EB | Elektrisch-Benzine
ED | Elektisch-Diesel
LPG | LPG/Gas
O | Overige

### transmission_type

Value | Description
----- | -----------
H | Handgeschakeld
A | Automaat
O | Overige / semi-automaat

### body_type

Value | Description
----- | -----------
HB | Hatchback
CB | Cabrio
CP | Coupe
SUV | SUV/Terreinwagen/Pick-up
SD | Sedan
SW | Stationwagon
MPV | MPV
CC | Bedrijfswagen (company car)
O | Overige

### mileage_type

Value | Description
----- | -----------
KM | Kilometer
M | Mijl

### engine_power_type

Value | Description
----- | -----------
PK | PK/HP
KW | KW

### engine_top_speed_type

Value | Description
----- | -----------
KM | KM/u
M | M/h

### images

The images key in the body should contain an array holding all images, a sample payload is:

```json
{
    // other data
    "images": [
        {
            "url": "http://www.google.com"
        },
        {
            "url": "http://www.google.com"
        },
        {
            "url": "http://www.google.com"
        }
    ]
    // other data
}
```

### videos

The videos key in the body should contain an array holding all images, including the video type, a sample payload is:

```json
{
    // other data
    "videos": [
        {
            "type": "YT",
            "url": "http://www.youtube.com"
        },
        {
            "type": "VM",
            "url": "http://www.vimeo.com"
        }
    ]
    // other data
}
```

Accepted video types currently are `YT` (YouTube) and `VM` (Vimeo).

### accessories

The accessories key should contain an array holding all accessories, a sample payload is:

```json
{
    // other data
    "accessories": ["xenon", "sportstoelen", "climate control"]
    // other data
}
```