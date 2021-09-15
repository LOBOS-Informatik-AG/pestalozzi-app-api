# Availability

## Get article (stock) availability

This endpoint allows you to get the stock information for an article

**URL** : `/stock-availability/:id`

This endpoint allows you also to get the stock information for an list of articles

**URL** : `/stock-availability/:id,:id,:id`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : Yes (HeaderParam: contactid)

**Permissions required** : No

**Query parameters** : Default filters

### Success Response

**Condition** : If storage location is found.

**Code** : `200 OK`

**Content example**

```json
[
    {
        "bIsCommercePartsList": false,
        "decQuantityAvailable": 0.000,
        "decQuantityAvailablePlan": 0.000,
        "decQuantityInProduction": null,
        "decQuantityOrdered": 0,
        "decQuantityReserved": 0,
        "decQuantityStockLevel": 0.000,
        "decReferenceQuantity": null,
        "decReplacementTime": null,
        "oStorageList": null,
        "sArticleID": "0101008H",
        "sQuantityUnit": "Stk",
        "sStorageGroupID": "",
        "shtStorageID": 1
    },
    ...
]
```

**or**

**Condition** : no storage locations are found for this article.

**Content example**

```json
{
    "text": "No stock information found"
}
```

## Post article (stock) availability

This endpoint allows you to get the stock information for a list of articles

**URL** : `/stock-availability/`

**Method** : <img src="https://img.shields.io/badge/POST%20-%23323330.svg?&style=flat&color=blue"/>

**Auth required** : Yes (HeaderParam: contactid)

**Permissions required** : No

**Body**

``` json
ID1,ID2,ID3
```

### Success Response

**Condition** : If storage location is found.

**Code** : `200 OK`

**Content example**

```json
[
    {
        "bIsCommercePartsList": false,
        "decQuantityAvailable": 0.000,
        "decQuantityAvailablePlan": 0.000,
        "decQuantityInProduction": null,
        "decQuantityOrdered": 0,
        "decQuantityReserved": 0,
        "decQuantityStockLevel": 0.000,
        "decReferenceQuantity": null,
        "decReplacementTime": null,
        "oStorageList": null,
        "sArticleID": "0101008H",
        "sQuantityUnit": "Stk",
        "sStorageGroupID": "",
        "shtStorageID": 1
    },
    ...
]
```

**or**

**Condition** : no storage locations are found for this article.

**Content example**

```json
{
    "text": "No stock information found"
}
```