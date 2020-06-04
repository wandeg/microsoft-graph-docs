---
title: "Update privilegedOperationEvent"
description: "Update the properties of a privilegedOperationEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privilegedOperationEvent
Namespace: microsoft.graph

Update the properties of a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

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
PATCH /privilegedOperationEvents/{privilegedOperationEventsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

The following table shows the properties that are required when you create the [privilegedOperationEvent](../resources/privilegedoperationevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userId|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|
|userMail|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|roleName|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|requestorId|String|**TODO: Add Description**|
|requestorName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|
|additionalInformation|String|**TODO: Add Description**|
|referenceKey|String|**TODO: Add Description**|
|referenceSystem|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privilegedoperationevent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedOperationEvents/{privilegedOperationEventsId}
Content-Type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "userId": "String",
  "userName": "String",
  "userMail": "String",
  "roleId": "String",
  "roleName": "String",
  "expirationDateTime": "String (timestamp)",
  "creationDateTime": "String (timestamp)",
  "requestorId": "String",
  "requestorName": "String",
  "tenantId": "String",
  "requestType": "String",
  "additionalInformation": "String",
  "referenceKey": "String",
  "referenceSystem": "String"
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
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "id": "144da38e-a38e-144d-8ea3-4d148ea34d14",
  "userId": "String",
  "userName": "String",
  "userMail": "String",
  "roleId": "String",
  "roleName": "String",
  "expirationDateTime": "String (timestamp)",
  "creationDateTime": "String (timestamp)",
  "requestorId": "String",
  "requestorName": "String",
  "tenantId": "String",
  "requestType": "String",
  "additionalInformation": "String",
  "referenceKey": "String",
  "referenceSystem": "String"
}
```

