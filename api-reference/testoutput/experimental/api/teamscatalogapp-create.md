---
title: "Create teamsCatalogApp"
description: "Create a new teamsCatalogApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsCatalogApp

Namespace: microsoft.graph

Create a new [teamsCatalogApp](../resources/teamscatalogapp.md) object.

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
POST /teams/{teamsId}/apps
POST /me/joinedGroups/{groupId}/team/apps
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [teamsCatalogApp](../resources/teamscatalogapp.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamscatalogapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/teams/{teamsId}/apps
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
  "truncated": true,
  "@odata.type": "microsoft.graph.teamscatalogapp"
}
-->
``` http
HTTP/1.1 201 Created
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

