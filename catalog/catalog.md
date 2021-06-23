# Catalog - Categories

## Get available categories

This endpoint allows you to get all the categories

**URL** : `/catalog-categories`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : No

**Permissions required** : No

**Query parameters** : No

### Success Response

**Condition** : If categories are found.

**Code** : `200 OK`

**Content example**

```json
[{...}]
```

Since the json file can be very large, use a suitable tool like wget to download it:
```
wget http://{{url}}/PL1APIHost/catalog-categories -O catalog-categories.json
```

**or**

**Condition** : no categories are found.

**Content example**

```json
{
    "text": "No categories found"
}
```

# Catalog - Articles

## Get available articles

This endpoint returns all items contained in the catalog

**URL** : `/catalog-articles`

**Method** : <img src="https://img.shields.io/badge/GET%20-%23323330.svg?&style=flat&color=green"/>

**Auth required** : No

**Permissions required** : No

**Query parameters** : No

### Success Response

**Condition** : If articles are found.

**Code** : `200 OK`

**Content example**

```json
[{...}]
```

Since the json file can be very large, use a suitable tool like wget to download it:
```
wget http://{{url}}/PL1APIHost/catalog-articles -O catalog-articles.json
```

**or**

**Condition** : no articles are found.

**Content example**

```json
{
    "text": "No categories found"
}
```