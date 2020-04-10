---
title: "Update publishedResource"
description: "Update the properties of a publishedResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update publishedResource

Namespace: microsoft.graph

Update the properties of a [publishedResource](../resources/publishedresource.md) object.

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
PATCH /onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/publishedResources/{publishedResourceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [publishedResource](../resources/publishedresource.md) object.

The following table shows the properties that are required when you create the [publishedResource](../resources/publishedresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|resourceName|String||
|publishingType|Enumeration| Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [publishedResource](../resources/publishedresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_publishedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{onPremisesPublishingProfilesId}/publishedResources/{publishedResourceId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.publishedResource",
  "displayName": "Display Name value",
  "resourceName": "Resource Name value",
  "publishingType": "String"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.publishedResource",
  "id": "bb8ff3a2-f3a2-bb8f-a2f3-8fbba2f38fbb",
  "displayName": "Display Name value",
  "resourceName": "Resource Name value",
  "publishingType": "String"
}
```

