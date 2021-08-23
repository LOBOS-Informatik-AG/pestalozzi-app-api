# Cart

## Create cart

This endpoint allows you to create a cart

**URL** : `/carts`

**Method** : <img src="https://img.shields.io/badge/POST%20-%23323330.svg?&style=flat&color=blue"/>

**Auth required** : Yes

**Permissions required** : No

**Body**

``` json
{
    "lngCartID": 7,
    "bGrossOrder": true,
    "dtDeliveryDate": 1603357783000,
    "dtEntryDate": 1603357783000,
    "dtAlterationDate": 1603357783000,
    "dtProcessingDate": 1603357783000,
    "dtSignDate": 1603357783000,
    "dtSubmitDate": 1603357783000,
    "decDiscountPercent1": 5,
    "decDiscountPercent2": 10,
    "decDiscountPercent3": 25,
    "decPackingCosts": 20,
    "decShippingCosts": 20,
    "decTotalGrossAmount": 2000,
    "decTotalNetAmount": 2000,
    "decTotalTaxAmount": 2000,
    "lngCustomerID": 23,
    "lngProjectID": 1,
    "lngContactID": 1,
    "lngSalesOrderID": 0,
    "lngTourID": 1,
    "DeliveryAddress": {
        "lngCustomerID": 31,
        "lngAddressID": 1,
        "id": 1,
        "shtAddressType": 1,
        "lngContactID": 8,
        "sContact": "Anouk_Lukoschek38@hotmail.com",
        "lngRouteBaseID": 1,
        "sCompany1": "Ertl - Balcer",
        "sCompany2": "Upgradable intermediate throughput",
        "sZipBox": "44331",
        "sPostBox": "PO Box",
        "sStreet": "66124 Elsa Freeway",
        "sZipCode": "56145",
        "sCity": "Janoscheid",
        "sCountry": "Seychellen",
        "sCountryCode": "EE"
    },
    "InvoiceAddress": {
        "lngCustomerID": 31,
        "lngAddressID": 1,
        "id": 1,
        "shtAddressType": 1,
        "lngContactID": 8,
        "sContact": "Anouk_Lukoschek38@hotmail.com",
        "lngRouteBaseID": 1,
        "sCompany1": "Ertl - Balcer",
        "sCompany2": "Upgradable intermediate throughput",
        "sZipBox": "44331",
        "sPostBox": "PO Box",
        "sStreet": "66124 Elsa Freeway",
        "sZipCode": "56145",
        "sCity": "Janoscheid",
        "sCountry": "Seychellen",
        "sCountryCode": "EE"
    },
    "sCartName": "My Cart 7",
    "sCartOrderType": "A",
    "sCurrencyCode": "CHF",
    "sDiscountText1": "",
    "sDiscountText2": "",
    "sDiscountText3": "",
    "sExtCartID": 0,
    "sForeignOrderID": 0,
    "sLanguageCode": "de",
    "sMemo": "",
    "sMemointernal": "",
    "sPayconnectionID": 1,
    "sPaymentID": 1,
    "sSalesOrderType": 1,
    "sSessionID": 1,
    "sUsername": "Danny.Willwacher@gmail.com",
    "sUserSign": "Danny.Willwacher@gmail.com",
    "sUserSubmit": "Danny.Willwacher@gmail.com",
    "shtCartStatus": 1,
    "shtPaymentConditionID": 1,
    "shtPaymentTypeID": 1,
    "shtShippingConditionID": 1,
    "shtWebshopID": 1
}
```

### Success Response

**Condition** : If the cart is successfully created.

**Code** : `200 OK`

**Content example**

```json
{
    ...
}
```
