---
title: "Create accessPackageResource"
description: "Create a new accessPackageResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackageResource

Namespace: microsoft.graph

Create a new [accessPackageResource](../resources/accesspackageresource.md) object.

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
POST /accessPackageResources
POST /identityGovernance/entitlementManagement/accessPackageResources
POST /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageResource](../resources/accesspackageresource.md) object.

The following table shows the properties that are required when you create the [accessPackageResource](../resources/accesspackageresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|url|String||
|resourceType|String||
|originId|String||
|originSystem|String||
|isPendingOnboarding|Boolean||
|addedBy|String||
|addedOn|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageResource](../resources/accesspackageresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresource_from_accesspackageresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageResources
Content-type: application/json
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
  "addedOn": "2017-01-01T00:02:37.1518445+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 447

{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "id": "e1baf168-f168-e1ba-68f1-bae168f1bae1",
  "displayName": "Display Name value",
  "description": "Description value",
  "url": "Url value",
  "resourceType": "Resource Type value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "isPendingOnboarding": true,
  "addedBy": "Added By value",
  "addedOn": "2017-01-01T00:02:37.1518445+00:00"
}
```

