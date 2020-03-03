---
title: "Create office365GroupsActivityCounts"
description: "Create a new office365GroupsActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365GroupsActivityCounts

Namespace: microsoft.graph

Create a new [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365GroupsActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object.

The following table shows the properties that are required when you create the [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|exchangeEmailsReceived|Int64||
|yammerMessagesPosted|Int64||
|yammerMessagesRead|Int64||
|yammerMessagesLiked|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365groupsactivitycounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365GroupsActivityCounts not found
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityCounts",
  "reportRefreshDate": "Date",
  "exchangeEmailsReceived": 6,
  "yammerMessagesPosted": 4,
  "yammerMessagesRead": 2,
  "yammerMessagesLiked": 3,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365groupsactivitycounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityCounts",
  "id": "75859bb3-9bb3-7585-b39b-8575b39b8575",
  "reportRefreshDate": "Date",
  "exchangeEmailsReceived": 6,
  "yammerMessagesPosted": 4,
  "yammerMessagesRead": 2,
  "yammerMessagesLiked": 3,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

