---
title: "List workbookFilters"
description: "List properties and relationships of the workbookFilter objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookFilters

List properties and relationships of the [workbookFilter](../resources/workbookfilter.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookFilter not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookFilter](../resources/workbookfilter.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookfilter"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.workbookFilter not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookfilter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 718

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookFilter",
      "id": "98dbf94e-f94e-98db-4ef9-db984ef9db98",
      "criteria": {
        "@odata.type": "microsoft.graph.workbookFilterCriteria",
        "color": "Color value",
        "criterion1": "Criterion1 value",
        "criterion2": "Criterion2 value",
        "dynamicCriteria": "Dynamic Criteria value",
        "filterOn": "Filter On value",
        "icon": {
          "@odata.type": "microsoft.graph.workbookIcon",
          "index": 5,
          "set": "Set value"
        },
        "operator": "Operator value",
        "values": {
          "@odata.type": "microsoft.graph.Json"
        }
      }
    }
  ]
}
```

