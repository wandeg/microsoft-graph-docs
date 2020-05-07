---
title: "Create sensitivityLabels"
description: "Create a new sensitivityLabels object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create sensitivityLabels

Namespace: microsoft.graph

Create a new sensitivityLabels object.

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
POST /dataClassification/sensitivityLabels
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [sensitivityLabel](../resources/sensitivitylabel.md) object.

The following table shows the properties that are required when you create the [sensitivityLabel](../resources/sensitivitylabel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|toolTip|String|**TODO: Add Description**|
|isEndpointProtectionEnabled|Boolean|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|applicationMode|applicationMode|**TODO: Add Description**. Possible values are: `manual`, `automatic`, `recommended`.|
|labelActions|[labelActionBase](../resources/labelactionbase.md) collection|**TODO: Add Description**|
|assignedPolicies|[labelPolicy](../resources/labelpolicy.md) collection|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|autoLabeling|[autoLabeling](../resources/autolabeling.md)|**TODO: Add Description**|
|applicableTo|sensitivityLabelTarget|**TODO: Add Description**. Possible values are: `email`, `site`, `unifiedGroup`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and a [sensitivityLabel](../resources/sensitivitylabel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_sensitivitylabel_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/sensitivityLabels
Content-Type: application/json
Content-length: 603

{
  "@odata.type": "#microsoft.graph.sensitivityLabel",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "toolTip": "String",
  "isEndpointProtectionEnabled": "Boolean",
  "isDefault": "Boolean",
  "applicationMode": "String",
  "labelActions": [
    {
      "@odata.type": "microsoft.graph.encryptWithUserDefinedRights"
    }
  ],
  "assignedPolicies": [
    {
      "@odata.type": "microsoft.graph.labelPolicy"
    }
  ],
  "priority": "Integer",
  "autoLabeling": {
    "@odata.type": "microsoft.graph.autoLabeling"
  },
  "applicableTo": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivitylabel"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.sensitivityLabel",
  "id": "ef55db95-db95-ef55-95db-55ef95db55ef",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "toolTip": "String",
  "isEndpointProtectionEnabled": "Boolean",
  "isDefault": "Boolean",
  "applicationMode": "String",
  "labelActions": [
    {
      "@odata.type": "microsoft.graph.encryptWithUserDefinedRights"
    }
  ],
  "assignedPolicies": [
    {
      "@odata.type": "microsoft.graph.labelPolicy"
    }
  ],
  "priority": "Integer",
  "autoLabeling": {
    "@odata.type": "microsoft.graph.autoLabeling"
  },
  "applicableTo": "String"
}
```

