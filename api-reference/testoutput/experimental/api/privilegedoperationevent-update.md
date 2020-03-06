---
title: "Update privilegedOperationEvent"
description: "Update the properties of a privilegedOperationEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedOperationEvent

Namespace: microsoft.graph

Update the properties of a [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.

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
PATCH /privilegedOperationEvents/{privilegedOperationEventsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedoperationevent"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/privilegedOperationEvents/{privilegedOperationEventsId}
Content-type: application/json
Content-length: 658

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "userId": "User Id value",
  "userName": "User Name value",
  "userMail": "User Mail value",
  "roleId": "Role Id value",
  "roleName": "Role Name value",
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00",
  "creationDateTime": "2016-12-31T23:59:35.5241957+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 707

{
  "@odata.type": "#microsoft.graph.privilegedOperationEvent",
  "id": "73676b3b-6b3b-7367-3b6b-67733b6b6773",
  "userId": "User Id value",
  "userName": "User Name value",
  "userMail": "User Mail value",
  "roleId": "Role Id value",
  "roleName": "Role Name value",
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00",
  "creationDateTime": "2016-12-31T23:59:35.5241957+03:00",
  "requestorId": "Requestor Id value",
  "requestorName": "Requestor Name value",
  "tenantId": "Tenant Id value",
  "requestType": "Request Type value",
  "additionalInformation": "Additional Information value",
  "referenceKey": "Reference Key value",
  "referenceSystem": "Reference System value"
}
```

