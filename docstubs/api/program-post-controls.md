---
title: "Add controls"
description: "Add controls by posting to the controls collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add controls

Namespace: microsoft.graph

Add controls by posting to the controls collection.

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
POST /programs/{programsId}/controls/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_programcontrol_from_programcontrols"
}
-->
``` http
POST https://graph.microsoft.com/beta/programs/{programsId}/controls
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
  "truncated": true,
  "@odata.type": "microsoft.graph.programcontrol"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 641

{
  "@odata.type": "#microsoft.graph.programControl",
  "id": "90d8f993-f993-90d8-93f9-d89093f9d890",
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
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00"
}
```

