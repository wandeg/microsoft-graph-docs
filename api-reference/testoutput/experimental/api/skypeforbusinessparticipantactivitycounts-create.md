---
title: "Create skypeForBusinessParticipantActivityCounts"
description: "Create a new skypeForBusinessParticipantActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create skypeForBusinessParticipantActivityCounts

Namespace: microsoft.graph

Create a new [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) object.

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
POST ** Collection URI for microsoft.graph.skypeForBusinessParticipantActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|audioVideo|Int64||
|appSharing|Int64||
|web|Int64||
|dialInOut3rdParty|Int64||
|reportRefreshDate|Date||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_skypeforbusinessparticipantactivitycounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.skypeForBusinessParticipantActivityCounts not found
Content-type: application/json
Content-length: 276

{
  "@odata.type": "#microsoft.graph.skypeForBusinessParticipantActivityCounts",
  "im": 2,
  "audioVideo": 10,
  "appSharing": 10,
  "web": 3,
  "dialInOut3rdParty": 1,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeforbusinessparticipantactivitycounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 325

{
  "@odata.type": "#microsoft.graph.skypeForBusinessParticipantActivityCounts",
  "id": "3c9a9d90-9d90-3c9a-909d-9a3c909d9a3c",
  "im": 2,
  "audioVideo": 10,
  "appSharing": 10,
  "web": 3,
  "dialInOut3rdParty": 1,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```

