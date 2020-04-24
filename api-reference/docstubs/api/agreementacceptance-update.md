---
title: "Update agreementAcceptance"
description: "Update the properties of an agreementAcceptance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update agreementAcceptance

Namespace: microsoft.graph

Update the properties of an [agreementAcceptance](../resources/agreementacceptance.md) object.

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
PATCH /agreementAcceptances/{agreementAcceptancesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [agreementAcceptance](../resources/agreementacceptance.md) object.

The following table shows the properties that are required when you create the [agreementAcceptance](../resources/agreementacceptance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|agreementId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|agreementFileId|String|**TODO: Add Description**|
|recordedDateTime|DateTimeOffset|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userEmail|String|**TODO: Add Description**|
|state|agreementAcceptanceState|**TODO: Add Description**. Possible values are: `accepted`, `declined`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [agreementAcceptance](../resources/agreementacceptance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_agreementacceptance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/agreementAcceptances/{agreementAcceptancesId}
Content-Type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "id": "63a0f9ec-f9ec-63a0-ecf9-a063ecf9a063",
  "agreementId": "Agreement Id value",
  "userId": "User Id value",
  "agreementFileId": "Agreement File Id value",
  "recordedDateTime": "2016-12-31T23:56:35.2919298+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userEmail": "User Email value",
  "state": "String"
}
```

