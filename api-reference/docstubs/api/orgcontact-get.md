---
title: "Get orgContact"
description: "Read the properties and relationships of an orgContact object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get orgContact

Namespace: microsoft.graph

Read the properties and relationships of an [orgContact](../resources/orgcontact.md) object.

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
If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}
-->
``` http
GET https://graph.microsoft.com/beta/contacts/{contactsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.orgContact",
    "id": "165a8813-8813-165a-1388-5a1613885a16",
    "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
    "addresses": [
      {
        "@odata.type": "microsoft.graph.physicalOfficeAddress",
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
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2017-01-01T00:01:31.6341616+03:00"
      }
    ],
    "phones": [
      {
        "@odata.type": "microsoft.graph.phone",
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

