---
title: "List templates"
description: "Get the synchronizationTemplates from the templates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List templates

Namespace: microsoft.graph

Get the synchronizationTemplates from the templates navigation property.

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
GET /applications/{applicationsId}/synchronization/templates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [synchronizationTemplate](../resources/synchronizationtemplate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/templates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.synchronizationtemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 534

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.synchronizationTemplate",
      "id": "64a0b35d-b35d-64a0-5db3-a0645db3a064",
      "applicationId": "23d4a478-a478-23d4-78a4-d42378a4d423",
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

