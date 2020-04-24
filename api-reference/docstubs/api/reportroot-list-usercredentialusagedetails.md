---
title: "List userCredentialUsageDetails"
description: "Get the userCredentialUsageDetails from the userCredentialUsageDetails navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List userCredentialUsageDetails

Namespace: microsoft.graph

Get the userCredentialUsageDetails from the userCredentialUsageDetails navigation property.

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
GET /reports/userCredentialUsageDetails
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
If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.usercredentialusagedetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
      "id": "49ff46b4-46b4-49ff-b446-ff49b446ff49",
      "feature": "String",
      "userPrincipalName": "User Principal Name value",
      "userDisplayName": "User Display Name value",
      "isSuccess": true,
      "authMethod": "String",
      "failureReason": "Failure Reason value",
      "eventDateTime": "2016-12-31T23:57:46.848839+03:00"
    }
  ]
}
```

