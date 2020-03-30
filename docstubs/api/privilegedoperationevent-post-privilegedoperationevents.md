---
title: "Create privilegedOperationEvent"
description: "Create a new privilegedOperationEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedOperationEvent

Namespace: microsoft.graph

Create a new [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

The following table shows the properties that are required when you create the [privilegedOperationEvent](../resources/privilegedoperationevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userId|String||
|userName|String||
|userMail|String||
|roleId|String||
|roleName|String||
|expirationDateTime|DateTimeOffset||
|creationDateTime|DateTimeOffset||
|requestorId|String||
|requestorName|String||
|tenantId|String||
|requestType|String||
|additionalInformation|String||
|referenceKey|String||
|referenceSystem|String||



## Response
If successful, this method returns a `201 Created` response code and a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedoperationevent_from_privilegedoperationevents"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedOperationEvents
Content-type: application/json
Content-length: 658

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "userId": "User Id value",
  "userName": "User Name value",
  "userMail": "User Mail value",
  "roleId": "Role Id value",
  "roleName": "Role Name value",
  "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
  "creationDateTime": "2016-12-31T23:57:30.6368517+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedoperationevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 707

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "id": "e202bd7a-bd7a-e202-7abd-02e27abd02e2",
  "userId": "User Id value",
  "userName": "User Name value",
  "userMail": "User Mail value",
  "roleId": "Role Id value",
  "roleName": "Role Name value",
  "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
  "creationDateTime": "2016-12-31T23:57:30.6368517+03:00",
  "requestorId": "Requestor Id value",
  "requestorName": "Requestor Name value",
  "tenantId": "Tenant Id value",
  "requestType": "Request Type value",
  "additionalInformation": "Additional Information value",
  "referenceKey": "Reference Key value",
  "referenceSystem": "Reference System value"
}
```

