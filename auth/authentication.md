# Authentication

Authentication is the verification of the credentials of the connection attempt. This process consists of sending the credentials from the remote access client to the remote access server in an either plaintext or encrypted form by using an authentication protocol.

## Login

This endpoint allows you to get a user by providing the user credentials

**URL** : `/auth/login/`

**Method** : <img src="https://img.shields.io/badge/POST%20-%23323330.svg?&style=flat&color=blue"/>

**Auth required** : No

**Permissions required** : None

**Body parameters**

The username and password field is required to successfully login

```json
{
    "username": "info@lobos.ch",
    "password": "xxxxxxxx"
}
```

### Success Response

**Condition** : If the login was successfull.

**Code** : `200 OK`

**Content example**

```json
{
    "oUser": {
        "dtLastLogin": 1601456845000,
        "dtRegistration": 1600249405000,
        "lngContactID": 95253,
        "lngCustomerID": 10010,
        "sEmail": "info@lobos.ch",
        "sFirstName": "Remo",
        "sFormOfAdress": "Herr",
        "sLastName": "Vetterli",
        "sMobilePhone": "",
        "sPhone": "",
        "sUserName": "info@lobos.ch",
        "shtLanguageID": 1
    }
}
```

### Error Responses

**Condition** : if the username or password aren't valid.

**Code** : `400 BAD REQUEST`

**Content example**

```json
{
    "text": "Ungültiges Passwort"
}

// or

{
    "text": "Benutzer ungültig"
}
```
