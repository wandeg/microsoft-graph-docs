---
title: "Update synchronizationTemplate"
description: "Update the properties of a synchronizationTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update synchronizationTemplate

Namespace: microsoft.graph

Update the properties of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.

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
PATCH /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [synchronizationTemplate](../resources/synchronizationtemplate.md) object.

The following table shows the properties that are required when you create the [synchronizationTemplate](../resources/synchronizationtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|applicationId|Guid||
|default|Boolean||
|description|String||
|discoverable|Boolean||
|factoryTag|String||
|metadata|[metadataEntry](../resources/metadataentry.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
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
```

