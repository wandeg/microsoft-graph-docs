---
title: "Create privilegedOperationEvent"
description: "Create a new privilegedOperationEvent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedOperationEvent

Namespace: microsoft.graph

Create a new [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

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
POST /privilegedOperationEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedoperationevent_from_privilegedoperationevents"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedOperationEvents
Content-Type: application/json
Content-length: 656

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "userId": "User Id value",
  "userName": "User Name value",
  "userMail": "User Mail value",
  "roleId": "Role Id value",
  "roleName": "Role Name value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "requestorId": "Requestor Id value",
  "requestorName": "Requestor Name value",
  "tenantId": "Tenant Id value",
  "requestType": "Request Type value",
  "additionalInformation": "Additional Information value",
  "referenceKey": "Reference Key value",
  "referenceSystem": "Reference System value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedoperationevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "id": "42789d05-9d05-4278-059d-7842059d7842",
  "userId": "User Id value",
  "userName": "User Name value",
  "userMail": "User Mail value",
  "roleId": "Role Id value",
  "roleName": "Role Name value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "requestorId": "Requestor Id value",
  "requestorName": "Requestor Name value",
  "tenantId": "Tenant Id value",
  "requestType": "Request Type value",
  "additionalInformation": "Additional Information value",
  "referenceKey": "Reference Key value",
  "referenceSystem": "Reference System value"
}
```

