---
title: "Get orgContact"
description: "Read properties and relationships of an orgContact object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get orgContact

Namespace: Microsoft.DirectoryServices

Read properties and relationships of an [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /contacts/{contactsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [orgContact](../resources/microsoft.directoryservices-orgcontact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}
-->
``` http
GET https://graph.microsoft.com/changelog/contacts/{contactsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.orgContact"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.orgContact",
    "id": "d45be9bb-e9bb-d45b-bbe9-5bd4bbe95bd4",
    "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
    "addresses": [
      {
        "@odata.type": "Microsoft.DirectoryServices.physicalOfficeAddress",
        "city": "City value",
        "countryOrRegion": "Country Or Region value",
        "officeLocation": "Office Location value",
        "postalCode": "Postal Code value",
        "state": "State value",
        "street": "Street value"
      }
    ],
    "companyName": "Company Name value",
    "department": "Department value",
    "displayName": "Display Name value",
    "givenName": "Given Name value",
    "jobTitle": "Job Title value",
    "mail": "Mail value",
    "mailNickname": "Mail Nickname value",
    "onPremisesSyncEnabled": true,
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2016-12-31T23:56:32.7107544+00:00"
      }
    ],
    "phones": [
      {
        "@odata.type": "Microsoft.DirectoryServices.phone",
        "type": "String",
        "number": "Number value"
      }
    ],
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "surname": "Surname value"
  }
}
```

