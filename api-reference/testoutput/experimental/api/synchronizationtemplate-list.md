---
title: "List synchronizationTemplates"
description: "List properties and relationships of the synchronizationTemplate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List synchronizationTemplates

Namespace: microsoft.graph

List properties and relationships of the [synchronizationTemplate](../resources/synchronizationtemplate.md) objects.

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
GET /applications/{applicationsId}/synchronization/templates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [synchronizationTemplate](../resources/synchronizationtemplate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}/synchronization/templates
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
      "id": "ef935b80-5b80-ef93-805b-93ef805b93ef",
      "applicationId": "c409845e-845e-c409-5e84-09c45e8409c4",
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

