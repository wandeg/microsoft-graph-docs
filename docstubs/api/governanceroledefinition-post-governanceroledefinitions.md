---
title: "Create governanceRoleDefinition"
description: "Create a new governanceRoleDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create governanceRoleDefinition

Namespace: microsoft.graph

Create a new [governanceRoleDefinition](../resources/governanceroledefinition.md) object.

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
POST /governanceRoleDefinitions
POST /privilegedAccess/{privilegedAccessId}/roleDefinitions
POST /governanceResources/{governanceResourcesId}/roleDefinitions
POST /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.

The following table shows the properties that are required when you create the [governanceRoleDefinition](../resources/governanceroledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceId|String||
|externalId|String||
|templateId|String||
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_governanceroledefinition_from_governanceroledefinitions"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleDefinitions
Content-type: application/json
Content-length: 220

{
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "resourceId": "Resource Id value",
  "externalId": "External Id value",
  "templateId": "Template Id value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceroledefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 269

{
  "@odata.type": "#microsoft.graph.governanceRoleDefinition",
  "id": "337a1f36-1f36-337a-361f-7a33361f7a33",
  "resourceId": "Resource Id value",
  "externalId": "External Id value",
  "templateId": "Template Id value",
  "displayName": "Display Name value"
}
```

