---
title: "Get userSecurityProfile"
description: "Read the properties and relationships of a userSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get userSecurityProfile

Namespace: microsoft.graph

Read the properties and relationships of a [userSecurityProfile](../resources/usersecurityprofile.md) object.

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
GET /Security/userSecurityProfiles/{userSecurityProfileId}
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

If successful, this method returns a `200 OK` response code and a [userSecurityProfile](../resources/usersecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_usersecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/userSecurityProfiles/{userSecurityProfileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.userSecurityProfile",
    "id": "c899f36f-f36f-c899-6ff3-99c86ff399c8",
    "accounts": [
      {
        "@odata.type": "microsoft.graph.userAccount"
      }
    ],
    "azureSubscriptionId": "String",
    "azureTenantId": "String",
    "createdDateTime": "String (timestamp)",
    "displayName": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "riskScore": "String",
    "tags": [
      "String"
    ],
    "userPrincipalName": "String",
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation"
    }
  }
}
```

