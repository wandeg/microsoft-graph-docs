---
title: "List templates"
description: "Get the synchronizationTemplates from the templates navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List templates

Namespace: microsoft.graph

Get the synchronizationTemplates from the templates navigation property.

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
GET /applications/{applicationsId}/synchronization/templates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [synchronizationTemplate](../resources/synchronizationtemplate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/templates
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.synchronizationtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.synchronizationTemplate",
      "id": "65cce3a8-e3a8-65cc-a8e3-cc65a8e3cc65",
      "applicationId": "fb10ed8a-ed8a-fb10-8aed-10fb8aed10fb",
      "default": true,
      "description": "Description value",
      "discoverable": true,
      "factoryTag": "Factory Tag value",
      "metadata": [
        {
          "@odata.type": "microsoft.graph.metadataEntry",
          "key": "Key value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

