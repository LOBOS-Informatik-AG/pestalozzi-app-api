# Shipping-Types

## Get available shipping-types

This endpoint allows you to get all the possible shipping-types

**URL** : `/shipping-types`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : No

**Permissions required** : No

**Query parameters** : No

### Success Response

**Condition** : If shipping-types are found.

**Code** : `200 OK`

**Content example**

```json
[
    {
        "bPL1ShopCollection": false,
        "bPL1ShopDelivery": true,
        "sName": "LKW",
        "shtShippingTypeID": 11
    },
    {
        "bPL1ShopCollection": false,
        "bPL1ShopDelivery": false,
        "sName": "Post",
        "shtShippingTypeID": 13
    },
    {
        "bPL1ShopCollection": false,
        "bPL1ShopDelivery": false,
        "sName": "Post Express",
        "shtShippingTypeID": 17
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Dietikon",
        "shtShippingTypeID": 51
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Zürich",
        "shtShippingTypeID": 52
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Jona",
        "shtShippingTypeID": 53
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Schaffhausen",
        "shtShippingTypeID": 54
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Aarau",
        "shtShippingTypeID": 55
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Rümlang",
        "shtShippingTypeID": 57
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Winterthur",
        "shtShippingTypeID": 58
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Gossau",
        "shtShippingTypeID": 59
    },
    {
        "bPL1ShopCollection": true,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Zug",
        "shtShippingTypeID": 60
    },
    {
        "bPL1ShopCollection": false,
        "bPL1ShopDelivery": false,
        "sName": "Abgeholt Uster",
        "shtShippingTypeID": 61
    }
]
```

**or**

**Condition** : no shipping-types are found.

**Content example**

```json
{
    "text": "No shipping-types found"
}
```