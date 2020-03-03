---
title: "parseExpression"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# parseExpression



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
POST /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/parseExpression
POST /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema/parseExpression
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
|expression|String||
|testInputObject|[expressionInputObject](../resources/expressionInputObject.md)||
|targetAttributeDefinition|[attributeDefinition](../resources/attributeDefinition.md)||



## Response
If successful, this action returns a `200 OK` response code and a [parseExpressionResponse](../resources/parseExpressionResponse.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/parseExpression

Content-type: application/json
Content-length: 1167

{
  "expression": "Expression value",
  "testInputObject": {
    "@odata.type": "microsoft.graph.expressionInputObject",
    "definition": {
      "@odata.type": "microsoft.graph.objectDefinition",
      "attributes": [
        {
          "@odata.type": "microsoft.graph.attributeDefinition",
          "anchor": true,
          "apiExpressions": [
            {
              "@odata.type": "microsoft.graph.stringKeyStringValuePair"
            }
          ],
          "caseExact": true,
          "multivalued": true,
          "mutability": "String",
          "referencedObjects": [
            {
              "@odata.type": "microsoft.graph.referencedObject",
              "referencedObjectName": "Referenced Object Name value",
              "referencedProperty": "Referenced Property value"
            }
          ]
        }
      ],
      "supportedApis": [
        "Supported Apis value"
      ]
    },
    "properties": [
      {
        "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
      }
    ]
  },
  "targetAttributeDefinition": {
    "@odata.type": "microsoft.graph.attributeDefinition"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseexpressionresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 85

{
  "value": {
    "@odata.type": "microsoft.graph.parseExpressionResponse"
  }
}
```

