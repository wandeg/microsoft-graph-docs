---
title: "Create accessPackageResource"
description: "Create a new accessPackageResource object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageResource

Namespace: microsoft.graph

Create a new [accessPackageResource](../resources/accesspackageresource.md) object.

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
POST /accessPackageResources
POST /identityGovernance/entitlementManagement/accessPackageResources
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageResource](../resources/accesspackageresource.md) object.

The following table shows the properties that are required when you create the [accessPackageResource](../resources/accesspackageresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|
|resourceType|String|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|
|isPendingOnboarding|Boolean|**TODO: Add Description**|
|addedBy|String|**TODO: Add Description**|
|addedOn|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageResource](../resources/accesspackageresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresource_from_accesspackageresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageResources
Content-Type: application/json
Content-length: 398

{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "displayName": "Display Name value",
  "description": "Description value",
  "url": "Url value",
  "resourceType": "Resource Type value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "isPendingOnboarding": true,
  "addedBy": "Added By value",
  "addedOn": "2016-12-31T23:57:56.5735419+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "id": "e8e4902b-902b-e8e4-2b90-e4e82b90e4e8",
  "displayName": "Display Name value",
  "description": "Description value",
  "url": "Url value",
  "resourceType": "Resource Type value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "isPendingOnboarding": true,
  "addedBy": "Added By value",
  "addedOn": "2016-12-31T23:57:56.5735419+03:00"
}
```

