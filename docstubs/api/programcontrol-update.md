---
title: "Update programControl"
description: "Update the properties of a programControl object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update programControl

Namespace: microsoft.graph

Update the properties of a [programControl](../resources/programcontrol.md) object.

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
PATCH /programControls/{programControlsId}
PATCH /programs/{programsId}/controls/{programControlId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [programControl](../resources/programcontrol.md) object.

The following table shows the properties that are required when you create the [programControl](../resources/programcontrol.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|controlId|String||
|programId|String||
|controlTypeId|String||
|displayName|String||
|status|String||
|owner|[userIdentity](../resources/useridentity.md)||
|resource|[programResource](../resources/programresource.md)||
|createdDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [programControl](../resources/programcontrol.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_programcontrol"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/programControls/{programControlsId}
Content-type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.programControl",
  "controlId": "Control Id value",
  "programId": "Program Id value",
  "controlTypeId": "Control Type Id value",
  "displayName": "Display Name value",
  "status": "Status value",
  "owner": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "resource": {
    "@odata.type": "microsoft.graph.programResource",
    "type": "Type value"
  }
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
Content-Length: 641

{
  "@odata.type": "#microsoft.graph.programControl",
  "id": "aabd7657-7657-aabd-5776-bdaa5776bdaa",
  "controlId": "Control Id value",
  "programId": "Program Id value",
  "controlTypeId": "Control Type Id value",
  "displayName": "Display Name value",
  "status": "Status value",
  "owner": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "resource": {
    "@odata.type": "microsoft.graph.programResource",
    "type": "Type value"
  },
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00"
}
```

