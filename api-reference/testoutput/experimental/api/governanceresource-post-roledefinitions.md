---
title: "Add roleDefinitions"
description: "Add roleDefinitions by posting to the roleDefinitions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add roleDefinitions

Add roleDefinitions by posting to the roleDefinitions collection.

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
POST /governanceResources/{governanceResourcesId}/roleDefinitions/$ref
POST /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the governanceRoleDefinition object.

The following table shows the properties that are required when you create the governanceRoleDefinition.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceId|String||
|externalId|String||
|templateId|String||
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_governanceroledefinition_from_governanceroledefinitions"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/governanceResources/{governanceResourcesId}/roleDefinitions
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
  "id": "060f2ae1-2ae1-060f-e12a-0f06e12a0f06",
  "resourceId": "Resource Id value",
  "externalId": "External Id value",
  "templateId": "Template Id value",
  "displayName": "Display Name value"
}
```

