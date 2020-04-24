---
title: "directoryDefinition: discover"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# discover

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /directories/{directoriesId}/discover
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [directoryDefinition](../resources/directorydefinition.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "directorydefinition_discover"
}
-->
``` http
POST https://graph.microsoft.com/beta/directories/{directoriesId}/discover
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorydefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.directoryDefinition",
    "id": "479269ef-69ef-4792-ef69-9247ef699247",
    "discoveryDateTime": "2016-12-31T23:57:06.5468887+03:00",
    "discoverabilities": "String",
    "name": "Name value",
    "objects": [
      {
        "@odata.type": "microsoft.graph.objectDefinition"
      }
    ],
    "readOnly": true,
    "version": "Version value"
  }
}
```

