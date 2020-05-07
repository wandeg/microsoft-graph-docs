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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
Content-length: 303

{
  "@odata.type": "#microsoft.graph.agreementAcceptance",
  "agreementId": "String",
  "userId": "String",
  "agreementFileId": "String",
  "recordedDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userEmail": "String",
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
  "id": "023bbdf4-bdf4-023b-f4bd-3b02f4bd3b02",
  "agreementId": "String",
  "userId": "String",
  "agreementFileId": "String",
  "recordedDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userEmail": "String",
  "state": "String"
}
```

