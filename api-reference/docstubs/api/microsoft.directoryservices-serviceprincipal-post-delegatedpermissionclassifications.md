---
title: "Create delegatedPermissionClassifications"
description: "Create a new delegatedPermissionClassifications object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create delegatedPermissionClassifications

Namespace: Microsoft.DirectoryServices

Create a new delegatedPermissionClassifications object.

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
POST /servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_delegatedpermissionclassification_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
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
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.delegatedpermissionclassification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.delegatedPermissionClassification",
  "id": "a92dc241-c241-a92d-41c2-2da941c22da9",
  "permissionId": "Permission Id value",
  "permissionName": "Permission Name value",
  "classification": "String"
}
```

