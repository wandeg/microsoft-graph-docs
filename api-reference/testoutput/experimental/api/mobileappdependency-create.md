---
title: "Create mobileAppDependency"
description: "Create a new mobileAppDependency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create mobileAppDependency

Namespace: microsoft.graph

Create a new [mobileAppDependency](../resources/mobileappdependency.md) object.

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
POST ** Collection URI for microsoft.graph.mobileAppDependency not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [mobileAppDependency](../resources/mobileappdependency.md) object.

The following table shows the properties that are required when you create the [mobileAppDependency](../resources/mobileappdependency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetId|String|The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|The target child mobile app's display name. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|dependencyType|Enumeration|The type of dependency relationship between the parent and child apps. Possible values are: `detect`, `autoInstall`.|
|dependentAppCount|Int32|The total number of dependencies the child app has.|



## Response
If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/mobileappdependency.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileappdependency_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.mobileAppDependency not found
Content-type: application/json
Content-length: 206

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "String",
  "dependentAppCount": 1
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileappdependency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 255

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "f862b777-b777-f862-77b7-62f877b762f8",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "String",
  "dependentAppCount": 1
}
```

