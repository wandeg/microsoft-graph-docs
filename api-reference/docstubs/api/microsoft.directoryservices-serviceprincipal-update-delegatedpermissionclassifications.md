---
title: "Update delegatedPermissionClassifications"
description: "Update the properties of a delegatedPermissionClassifications object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update delegatedPermissionClassifications

Namespace: Microsoft.DirectoryServices

Update the properties of a delegatedPermissionClassifications object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md) object.

The following table shows the properties that are required when you create the [delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|permissionId|String|**TODO: Add Description**|
|permissionName|String|**TODO: Add Description**|
|classification|permissionClassificationType|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_delegatedpermissionclassifications"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
Content-Type: application/json
Content-length: 206

{
  "@odata.type": "#Microsoft.DirectoryServices.delegatedPermissionClassification",
  "permissionId": "Permission Id value",
  "permissionName": "Permission Name value",
  "classification": "String"
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
{
  "@odata.type": "#Microsoft.DirectoryServices.delegatedPermissionClassification",
  "id": "a92dc241-c241-a92d-41c2-2da941c22da9",
  "permissionId": "Permission Id value",
  "permissionName": "Permission Name value",
  "classification": "String"
}
```

