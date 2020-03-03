---
title: "Create userTeamwork"
description: "Create a new userTeamwork object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create userTeamwork

Namespace: microsoft.graph

Create a new [userTeamwork](../resources/userteamwork.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.userTeamwork not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [userTeamwork](../resources/userteamwork.md) object.

The following table shows the properties that are required when you create the [userTeamwork](../resources/userteamwork.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [userTeamwork](../resources/userteamwork.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_userteamwork_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.userTeamwork not found
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.userTeamwork"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userteamwork"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.userTeamwork",
  "id": "47ac7302-7302-47ac-0273-ac470273ac47"
}
```

