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
|Authorization|Bearer {token}. Required.|

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
    "id": "38669964-9964-3866-6499-663864996638",
    "deletedDateTime": "String (timestamp)",
    "addresses": [
      {
        "@odata.type": "microsoft.graph.physicalOfficeAddress"
      }
    ],
    "companyName": "String",
    "department": "String",
    "displayName": "String",
    "givenName": "String",
    "jobTitle": "String",
    "mail": "String",
    "mailNickname": "String",
    "onPremisesSyncEnabled": "Boolean",
    "onPremisesLastSyncDateTime": "String (timestamp)",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError"
      }
    ],
    "phones": [
      {
        "@odata.type": "microsoft.graph.phone"
      }
    ],
    "proxyAddresses": [
      "String"
    ],
    "surname": "String"
  }
}
```

