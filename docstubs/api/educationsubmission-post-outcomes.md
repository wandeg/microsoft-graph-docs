---
title: "Add outcomes"
description: "Add outcomes by posting to the outcomes collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add outcomes

Namespace: microsoft.graph

Add outcomes by posting to the outcomes collection.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/outcomes/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationOutcome](../resources/educationoutcome.md) object.

The following table shows the properties that are required when you create the [educationOutcome](../resources/educationoutcome.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [educationOutcome](../resources/educationoutcome.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationoutcome_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/outcomes
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.educationOutcome"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationoutcome"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 544

{
  "@odata.type": "#microsoft.graph.educationOutcome",
  "id": "5501a8f3-a8f3-5501-f3a8-0155f3a80155",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
}
```

