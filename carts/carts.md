# Cart

## Get carts

This endpoint allows you to get the carts for the authenticated user

**URL** : `/carts`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : Yes

**Permissions required** : No

**Query parameters** : Default filters

### Success Response

**Condition** : If carts are found.

**Code** : `200 OK`

**Content example**

```json
[
    ...
]
```

**or**

**Condition** : no carts have been found.

**Content example**

```json
{
  "text": "Keine Warenkörbe gefunden."
}
```

## Get cart by id

This endpoint allows you to get a cart by id

**URL** : `/carts/:id`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : Yes

**Permissions required** : No

### Success Response

**Condition** : If the cart is found.

**Code** : `200 OK`

**Content example**

```json
{
    ...
}
```

**or**

**Condition** : if no cart is found.

**Content example**

```json
{
    "text": "Kein Warenkorb gefunden"
}
```

## Create cart

This endpoint allows you to create a cart

**URL** : `/carts`

**Method** : <img src="https://img.shields.io/badge/POST%20-%23323330.svg?&style=flat&color=blue"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
{
    "sCartName": "Neuer Warenkorb PPE",
    "shtStatus": 0
}
```

### Success Response

**Condition** : If the cart is successfully created.

**Code** : `200 OK`

**Content example**

```json
{
    "bGrossOrder": null,
    "decDiscountPercent1": 5,
    "decDiscountPercent2": 10,
    "decDiscountPercent3": 25,
    "decPackingCosts": 20,
    "decShippingCosts": 20,
    "decTotalGrossAmount": 2000,
    "decTotalNetAmount": 2000,
    "decTotalTaxAmount": 2000,
    "dtAlterationDate": 1629713713000,
    "dtDeliveryDate": 1603357783000,
    "dtEntryDate": 1629713713000,
    "dtP48DateRequested": null,
    "dtProcessingDate": 1603357783000,
    "dtSignDate": 1603357783000,
    "dtSubmitDate": 1603357783000,
    "lngCartID": 20210816267,
    "lngContactID": 1,
    "lngCustomerID": 23,
    "lngProjectID": 1,
    "lngSalesOrderID": 0,
    "lngTourID": null,
    "oCartItemList": null,
    "oDeliveryAddress": {
        "sCity": "",
        "sCompany1": "",
        "sCompany2": "",
        "sContact": "",
        "sCountry": "",
        "sCountryCode": "",
        "sPostBox": "",
        "sStreet": "",
        "sZipBox": "",
        "sZipCode": ""
    },
    "oInvoiceAddress": {
        "sCity": "",
        "sCompany1": "",
        "sCompany2": "",
        "sContact": "",
        "sCountry": "",
        "sCountryCode": "",
        "sPostBox": "",
        "sStreet": "",
        "sZipBox": "",
        "sZipCode": ""
    },
    "sCartName": "My Cart 7",
    "sCartOrderType": "A",
    "sContactName": "",
    "sCurrencyCode": "",
    "sDiscountText1": "",
    "sDiscountText2": "",
    "sDiscountText3": "",
    "sEmail": "",
    "sExtCartID": "0",
    "sForeignOrderID": "0",
    "sLanguageCode": "de",
    "sMemo": "",
    "sMemointernal": "",
    "sPayconnectionID": "",
    "sPaymentID": "1",
    "sSalesOrderType": "1",
    "sSessionID": "1",
    "sUserSign": "Danny.Willwacher@gmail.com",
    "sUserSubmit": "Danny.Willwacher@gmail.com",
    "sUsername": "ppellegrino@lobos.ch",
    "shtCartStatus": 1,
    "shtPaymentConditionID": 1,
    "shtPaymentTypeID": 1,
    "shtShippingConditionID": 1
}
```
## Update cart

This endpoint allows you to update a cart

**URL** : `/carts/:id`

**Method** : <img src="https://img.shields.io/badge/PUT%20-%23323330.svg?&style=flat&color=yellow"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
{
    ...
}
```

### Success Response

**Condition** : If the cart is successfully updated.

**Code** : `200 OK`

**Content example**

```json
{
    ...
}
```

## Delete cart

This endpoint allows you to delete a cart

**URL** : `/carts/:id`

**Method** : <img src="https://img.shields.io/badge/DELETE%20-%23323330.svg?&style=flat&color=red"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
None
```

### Success Response

**Condition** : If the cart is deleted successfully.

**Code** : `200 OK`

**Content example**

```json
None
```
## Get cart-items

This endpoint allows you to get all the cart-items

**URL** : `/carts/:id/items`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : Yes

**Permissions required** : No

**Query parameters** : Default filters

### Success Response

**Condition** : If cart-items are found.

**Code** : `200 OK`

**Content example**

```json
[
    ...
]
```

**or**

**Condition** : no cart-items are found.

**Content example**

```json
{
    "text": "Keine Warenkorbpositionen gefunden."
}
```
## Create cart-item

This endpoint allows you create a cart-item

**URL** : `/carts/:id/items`

**Method** : <img src="https://img.shields.io/badge/POST%20-%23323330.svg?&style=flat&color=blue"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
{

        "sArticleID": "32113000010000004000",
        "sQuantityUnit": "SK",
        "decQutantity": 4
}
```

### Success Response

**Condition** : If the item is succesfully created.

**Code** : `200 OK`

**Content example**

```json
{
    "decItemGrossAmount": 13.00,
    "decItemNetAmount": 13.00,
    "decItemTaxAmount": 0,
    "decPriceFactor": null,
    "decQuantity": 7.000,
    "decSalesPrice": 2.65,
    "decTaxRate": null,
    "lngCartID": 20210816267,
    "lngSalesPriceUnit": 1,
    "oArticle": null,
    "oDiscount1": {
        "decDiscountAmount": 0,
        "decDiscountPercent": 30.00,
        "decDiscountValue": 5.57,
        "lngDiscountID": 661316,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": "K"
    },
    "oDiscount2": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount3": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount4": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount5": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount6": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "sArticleID": "32113000010000004000",
    "sArticleName": "7001  15 Bogen 90°",
    "sExtItemID": "",
    "sItemText": "",
    "sQuantityUnit": "SK",
    "shtCartDetailStatus": 2,
    "shtHasAdditionalItems": null,
    "shtItemID": 1,
    "shtQuantityUnit": null
}
```

## Create cart-items

This endpoint allows you create cart-items (bulk)

**URL** : `/carts/:id/items/all`

**Method** : <img src="https://img.shields.io/badge/POST%20-%23323330.svg?&style=flat&color=blue"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
[
    {

            "sArticleID": "32113000010000004000",
            "sQuantityUnit": "SK",
            "decQutantity": 1
    },
    {

            "sArticleID": "32113000010000004000",
            "sQuantityUnit": "SK",
            "decQutantity": 2
    },
    {

            "sArticleID": "32113000010000004000",
            "sQuantityUnit": "SK",
            "decQutantity": 4
    }
]
```

### Success Response

**Condition** : If the item is succesfully created.

**Code** : `200 OK`

**Content example**

```json
{
    "decItemGrossAmount": 13.00,
    "decItemNetAmount": 13.00,
    "decItemTaxAmount": 0,
    "decPriceFactor": null,
    "decQuantity": 7.000,
    "decSalesPrice": 2.65,
    "decTaxRate": null,
    "lngCartID": 20210816267,
    "lngSalesPriceUnit": 1,
    "oArticle": null,
    "oDiscount1": {
        "decDiscountAmount": 0,
        "decDiscountPercent": 30.00,
        "decDiscountValue": 5.57,
        "lngDiscountID": 661316,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": "K"
    },
    "oDiscount2": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount3": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount4": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount5": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "oDiscount6": {
        "decDiscountAmount": null,
        "decDiscountPercent": 0.00,
        "decDiscountValue": null,
        "lngDiscountID": null,
        "sDiscountFlag": "",
        "sDiscountText": "",
        "sDiscountType": ""
    },
    "sArticleID": "32113000010000004000",
    "sArticleName": "7001  15 Bogen 90°",
    "sExtItemID": "",
    "sItemText": "",
    "sQuantityUnit": "SK",
    "shtCartDetailStatus": 2,
    "shtHasAdditionalItems": null,
    "shtItemID": 1,
    "shtQuantityUnit": null
}
```

## Update cart-item

This endpoint allows you to update a item

**URL** : `/carts/:id/items/:id`

**Method** : <img src="https://img.shields.io/badge/PUT%20-%23323330.svg?&style=flat&color=yellow"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
{
    ...
}
```

### Success Response

**Condition** : If the cart is updated successfully.

**Code** : `200 OK`

**Content example**

```json
{
    ...
}
```

## Delete cart-item

This endpoint allows you to delete a cart-item

**URL** : `/carts/:id/items/:id`

**Method** : <img src="https://img.shields.io/badge/DELETE%20-%23323330.svg?&style=flat&color=red"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
None
```

### Success Response

**Condition** : If the cart-item is deleted successfully.

**Code** : `200 OK`

**Content example**

```json
None
```
## Submit carts

This endpoint allows you to submit a cart

**URL** : `/carts/:id/submit`

**Method** : <img src="https://img.shields.io/badge/PUT%20-%23323330.svg?&style=flat&color=yellow"/>

**Auth required** : Yes

**Permissions required** : No

### Success Response

**Condition** : If carts are found and submitted.

**Code** : `200 OK`

**Content example**

```json
{
  "errorLevel": 2,
  "text": "Warenkorb angelegt"
}
```

**or**

**Condition** : cart allready submitted.

**Code** : `500 Internal Server Error`

**Content example**

```json
{
    "errorLevel": 2,
    "text": "Warenkorb bereits versendet"
}
```

**or**

**Condition** : no cart found.

**Code** : `200 OK`

**Content example**

```json
{
    "errorLevel": 2,
    "text": "Warenkorb nicht gefunden"
}
```
