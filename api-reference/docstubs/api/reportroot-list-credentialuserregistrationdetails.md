---
title: "List credentialUserRegistrationDetails"
description: "Get the credentialUserRegistrationDetails from the credentialUserRegistrationDetails navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List credentialUserRegistrationDetails

Namespace: microsoft.graph

Get the credentialUserRegistrationDetails from the credentialUserRegistrationDetails navigation property.

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
GET /reports/credentialUserRegistrationDetails
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
If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.credentialuserregistrationdetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
      "id": "211e4482-4482-211e-8244-1e2182441e21",
      "userPrincipalName": "User Principal Name value",
      "userDisplayName": "User Display Name value",
      "authMethods": [
        "String"
      ],
      "isRegistered": true,
      "isEnabled": true,
      "isCapable": true,
      "isMfaRegistered": true
    }
  ]
}
```

