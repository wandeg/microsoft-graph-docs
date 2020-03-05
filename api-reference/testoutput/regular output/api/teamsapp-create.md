---
title: "Create teamsApp"
description: "Create a new teamsApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsApp

Namespace: microsoft.graph

Create a new [teamsApp](../resources/teamsapp.md) object.

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
POST /appCatalogs/teamsApps
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [teamsApp](../resources/teamsapp.md) object.

The following table shows the properties that are required when you create the [teamsApp](../resources/teamsapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|displayName|String||
|distributionMethod|Enumeration|. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [teamsApp](../resources/teamsapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/appCatalogs/teamsApps
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "fabc42d6-42d6-fabc-d642-bcfad642bcfa",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "distributionMethod": "String"
}
```

