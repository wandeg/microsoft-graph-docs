---
title: "Create sharePointActivityPages"
description: "Create a new sharePointActivityPages object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sharePointActivityPages

Create a new [sharePointActivityPages](../resources/sharepointactivitypages.md) object.

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
POST ** Collection URI for microsoft.graph.sharePointActivityPages not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the sharePointActivityPages object.

The following table shows the properties that are required when you create the sharePointActivityPages.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|visitedPageCount|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [sharePointActivityPages](../resources/sharepointactivitypages.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sharepointactivitypages_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.sharePointActivityPages not found
Content-type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.sharePointActivityPages",
  "reportRefreshDate": "Date",
  "visitedPageCount": 0,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharepointactivitypages"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 239

{
  "@odata.type": "#microsoft.graph.sharePointActivityPages",
  "id": "8d696e93-6e93-8d69-936e-698d936e698d",
  "reportRefreshDate": "Date",
  "visitedPageCount": 0,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

