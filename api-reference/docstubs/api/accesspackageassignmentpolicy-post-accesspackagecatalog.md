---
title: "Create accessPackageCatalog"
description: "Create a new accessPackageCatalog object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageCatalog

Namespace: microsoft.graph

Create a new accessPackageCatalog object.

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
POST /accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}/accessPackageCatalog
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

The following table shows the properties that are required when you create the [accessPackageCatalog](../resources/accesspackagecatalog.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|catalogType|String|**TODO: Add Description**|
|catalogStatus|String|**TODO: Add Description**|
|isExternallyVisible|Boolean|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}/accessPackageCatalog
Content-Type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "displayName": "Display Name value",
  "description": "Description value",
  "catalogType": "Catalog Type value",
  "catalogStatus": "Catalog Status value",
  "isExternallyVisible": true,
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackagecatalog"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "ed0dcd9e-cd9e-ed0d-9ecd-0ded9ecd0ded",
  "displayName": "Display Name value",
  "description": "Description value",
  "catalogType": "Catalog Type value",
  "catalogStatus": "Catalog Status value",
  "isExternallyVisible": true,
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00"
}
```

