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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [threatAssessmentResult](../resources/threatassessmentresult.md) object.

The following table shows the properties that are required when you create the [threatAssessmentResult](../resources/threatassessmentresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|resultType|Enumeration| Possible values are: `checkPolicy`, `rescan`, `unknownFutureValue`.|
|message|String||



## Response
If successful, this method returns a `201 Created` response code and a [threatAssessmentResult](../resources/threatassessmentresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_threatassessmentresult_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "resultType": "String",
  "message": "Message value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatassessmentresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "id": "88de20c2-20c2-88de-c220-de88c220de88",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "resultType": "String",
  "message": "Message value"
}
```

