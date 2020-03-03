---
title: "Update teamsCatalogApp"
description: "Update the properties of a teamsCatalogApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsCatalogApp

Namespace: microsoft.graph

Update the properties of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.

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
PATCH /teams/{teamsId}/apps/{teamsCatalogAppId}
PATCH /me/joinedGroups/{groupId}/team/apps/{teamsCatalogAppId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsCatalogApp](../resources/teamscatalogapp.md) object.

The following table shows the properties that are required when you create the [teamsCatalogApp](../resources/teamscatalogapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|name|String||
|distributionMethod|Enumeration|. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsCatalogApp](../resources/teamscatalogapp.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamscatalogapp"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/teams/{teamsId}/apps/{teamsCatalogAppId}
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "externalId": "External Id value",
  "name": "Name value",
  "distributionMethod": "String"
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
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "id": "11dd4ded-4ded-11dd-ed4d-dd11ed4ddd11",
  "externalId": "External Id value",
  "name": "Name value",
  "distributionMethod": "String"
}
```

