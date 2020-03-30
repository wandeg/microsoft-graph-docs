---
title: "Add templates"
description: "Add templates by posting to the templates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add templates

Namespace: microsoft.graph

Add templates by posting to the templates collection.

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
POST /applications/{applicationsId}/synchronization/templates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/templates
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
  "applicationId": "8c1f5487-5487-8c1f-8754-1f8c87541f8c",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationtemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
  "id": "cb65ebcc-ebcc-cb65-cceb-65cbcceb65cb",
  "applicationId": "8c1f5487-5487-8c1f-8754-1f8c87541f8c",
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

