---
title: "Create delegatedPermissionClassification"
description: "Create a new delegatedPermissionClassification object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create delegatedPermissionClassification

Create a new [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

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
POST ** Collection URI for microsoft.graph.delegatedPermissionClassification not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the delegatedPermissionClassification object.

The following table shows the properties that are required when you create the delegatedPermissionClassification.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|permissionId|String||
|permissionName|String||
|classification|Enumeration|. Possible values are: `low`, `medium`, `high`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_delegatedpermissionclassification_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.delegatedPermissionClassification not found
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
  "permissionId": "Permission Id value",
  "permissionName": "Permission Name value",
  "classification": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedpermissionclassification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
  "id": "947f692a-692a-947f-2a69-7f942a697f94",
  "permissionId": "Permission Id value",
  "permissionName": "Permission Name value",
  "classification": "String"
}
```

