---
title: "evaluateClassificationResults"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# evaluateClassificationResults



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
POST /informationProtection/policy/labels/evaluateClassificationResults
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|contentInfo|[contentInfo](../resources/contentInfo.md)||
|classificationResults|[classificationResult](../resources/classificationResult.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [informationProtectionAction](../resources/informationProtectionAction.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/informationProtection/policy/labels/evaluateClassificationResults

Content-type: application/json
Content-length: 305

{
  "contentInfo": {
    "@odata.type": "microsoft.graph.contentInfo"
  },
  "classificationResults": [
    {
      "@odata.type": "microsoft.graph.classificationResult",
      "sensitiveTypeId": "01f68005-8005-01f6-0580-f6010580f601",
      "count": 5,
      "confidenceLevel": 15
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.informationprotectionaction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 100

{
  "value": [
    {
      "@odata.type": "microsoft.graph.addContentFooterAction"
    }
  ]
}
```

