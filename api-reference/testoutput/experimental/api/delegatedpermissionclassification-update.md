---
title: "Update delegatedPermissionClassification"
description: "Update the properties of a delegatedPermissionClassification object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update delegatedPermissionClassification

Namespace: microsoft.graph

Update the properties of a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

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
PATCH ** Entity URI for microsoft.graph.delegatedPermissionClassification not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

The following table shows the properties that are required when you create the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|permissionId|String||
|permissionName|String||
|classification|Enumeration|. Possible values are: `low`, `medium`, `high`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_delegatedpermissionclassification"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.delegatedPermissionClassification not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
  "id": "68614311-4311-6861-1143-616811436168",
  "permissionId": "Permission Id value",
  "permissionName": "Permission Name value",
  "classification": "String"
}
```

