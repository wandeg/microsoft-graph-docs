---
title: "Add results"
description: "Add results by posting to the results collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add results

Namespace: microsoft.graph

Add results by posting to the results collection.

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
POST /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [threatAssessmentResult](../resources/threatassessmentresult.md) object.

The following table shows the properties that are required when you create the [threatAssessmentResult](../resources/threatassessmentresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|resultType|Enumeration|. Possible values are: `checkPolicy`, `rescan`, `unknownFutureValue`.|
|message|String||



## Response
If successful, this method returns a `201 Created` response code and a [threatAssessmentResult](../resources/threatassessmentresult.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_threatassessmentresult_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "resultType": "String",
  "message": "Message value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatassessmentresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "id": "547f34d2-34d2-547f-d234-7f54d2347f54",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "resultType": "String",
  "message": "Message value"
}
```

