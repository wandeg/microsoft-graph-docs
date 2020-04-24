---
title: "Create parent"
description: "Create a new parent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create parent

Namespace: microsoft.graph

Create a new parent object.

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
POST /governanceResources/{governanceResourcesId}/parent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [governanceResource](../resources/governanceresource.md) object.

The following table shows the properties that are required when you create the [governanceResource](../resources/governanceresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|externalId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|registeredDateTime|DateTimeOffset|**TODO: Add Description**|
|registeredRoot|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [governanceResource](../resources/governanceresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governanceresource_from_governanceresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceResources/{governanceResourcesId}/parent
Content-Type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2017-01-01T00:00:25.9110048+03:00",
  "registeredRoot": "Registered Root value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.governanceResource",
  "id": "9740a6cb-a6cb-9740-cba6-4097cba64097",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2017-01-01T00:00:25.9110048+03:00",
  "registeredRoot": "Registered Root value"
}
```

