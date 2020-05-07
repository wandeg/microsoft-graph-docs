---
title: "Get synchronizationTemplate"
description: "Read the properties and relationships of a synchronizationTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get synchronizationTemplate

Namespace: microsoft.graph

Read the properties and relationships of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.

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
GET /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

