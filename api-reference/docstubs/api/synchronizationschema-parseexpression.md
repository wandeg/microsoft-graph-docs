---
title: "synchronizationSchema: parseExpression"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# parseExpression

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/parseExpression
POST /applications/{applicationsId}/synchronization/templates/{synchronizationTemplateId}/schema/parseExpression
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|expression|String|**TODO: Add Description**|
|testInputObject|[expressionInputObject](../resources/expressioninputobject.md)|**TODO: Add Description**|
|targetAttributeDefinition|[attributeDefinition](../resources/attributedefinition.md)|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [parseExpressionResponse](../resources/parseexpressionresponse.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}/schema/parseExpression

Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseexpressionresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "microsoft.graph.parseExpressionResponse"
  }
}
```

