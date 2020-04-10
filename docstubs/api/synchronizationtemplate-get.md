---
title: "Get synchronizationTemplate"
description: "Read properties and relationships of the synchronizationTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get synchronizationTemplate

Namespace: microsoft.graph

Read properties and relationships of the [synchronizationTemplate](../resources/synchronizationtemplate.md) object.

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
GET /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}
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
If successful, this method returns a `200 OK` response code and [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.

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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": {
    "@odata.type": "#microsoft.graph.synchronizationTemplate",
    "id": "d81009c1-09c1-d810-c109-10d8c10910d8",
    "applicationId": "20bc43e2-43e2-20bc-e243-bc20e243bc20",
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
}
```

