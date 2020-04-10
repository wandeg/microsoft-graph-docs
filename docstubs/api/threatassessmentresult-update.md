---
title: "Update threatAssessmentResult"
description: "Update the properties of a threatAssessmentResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update threatAssessmentResult

Namespace: microsoft.graph

Update the properties of a [threatAssessmentResult](../resources/threatassessmentresult.md) object.

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
PATCH /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/{threatAssessmentResultId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [threatAssessmentResult](../resources/threatassessmentresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_threatassessmentresult"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/{threatAssessmentResultId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

