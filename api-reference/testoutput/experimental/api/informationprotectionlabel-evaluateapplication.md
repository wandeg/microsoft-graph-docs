---
title: "evaluateApplication"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# evaluateApplication



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
POST /informationProtection/policy/labels/evaluateApplication
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
|labelingOptions|[labelingOptions](../resources/labelingOptions.md)||



## Response
If successful, this action returns a `200 OK` response code and a [informationProtectionAction](../resources/informationProtectionAction.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/informationProtection/policy/labels/evaluateApplication

Content-type: application/json
Content-length: 532

{
  "contentInfo": {
    "@odata.type": "microsoft.graph.contentInfo"
  },
  "labelingOptions": {
    "@odata.type": "microsoft.graph.labelingOptions",
    "labelId": "b2acd3da-d3da-b2ac-dad3-acb2dad3acb2",
    "downgradeJustification": {
      "@odata.type": "microsoft.graph.downgradeJustification",
      "justificationMessage": "Justification Message value",
      "isDowngradeJustified": true
    },
    "extendedProperties": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ]
  }
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

