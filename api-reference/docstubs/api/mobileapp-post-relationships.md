---
title: "Add relationships"
description: "Add relationships by posting to the relationships collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add relationships

Namespace: microsoft.graph

Add relationships by posting to the relationships collection.

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppRelationship](../resources/mobileapprelationship.md) object.

The following table shows the properties that are required when you create the [mobileAppRelationship](../resources/mobileapprelationship.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetId|String||
|targetDisplayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [mobileAppRelationship](../resources/mobileapprelationship.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileapprelationship_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileapprelationship"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "6736022b-022b-6736-2b02-36672b023667",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value"
}
```

