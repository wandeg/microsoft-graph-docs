---
title: "Update templates"
description: "Update the properties of a templates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update templates

Namespace: microsoft.graph

Update the properties of a templates object.

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
PATCH /applications/{applicationsId}/synchronization/templates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [synchronizationTemplate](../resources/synchronizationtemplate.md) object.

The following table shows the properties that are required when you create the [synchronizationTemplate](../resources/synchronizationtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|applicationId|Guid|**TODO: Add Description**|
|default|Boolean|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discoverable|Boolean|**TODO: Add Description**|
|factoryTag|String|**TODO: Add Description**|
|metadata|[metadataEntry](../resources/metadataentry.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_templates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/templates
Content-Type: application/json
Content-length: 294

{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
  "applicationId": "Guid",
  "default": "Boolean",
  "description": "String",
  "discoverable": "Boolean",
  "factoryTag": "String",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.metadataEntry"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
  "id": "c04b8792-8792-c04b-9287-4bc092874bc0",
  "applicationId": "Guid",
  "default": "Boolean",
  "description": "String",
  "discoverable": "Boolean",
  "factoryTag": "String",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.metadataEntry"
    }
  ]
}
```

