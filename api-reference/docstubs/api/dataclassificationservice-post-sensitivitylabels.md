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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
Content-length: 950

{
  "@odata.type": "#microsoft.graph.sensitivityLabel",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "toolTip": "Tool Tip value",
  "isEndpointProtectionEnabled": true,
  "isDefault": true,
  "applicationMode": "String",
  "labelActions": [
    {
      "@odata.type": "microsoft.graph.encryptWithUserDefinedRights",
      "encryptWith": "String",
      "decryptionRightsManagementTemplateId": "Decryption Rights Management Template Id value",
      "allowMailForwarding": true,
      "allowAdHocPermissions": true
    }
  ],
  "assignedPolicies": [
    {
      "@odata.type": "microsoft.graph.labelPolicy",
      "id": "Id value"
    }
  ],
  "priority": 8,
  "autoLabeling": {
    "@odata.type": "microsoft.graph.autoLabeling",
    "sensitiveTypeIds": [
      "Sensitive Type Ids value"
    ],
    "message": "Message value"
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
  "id": "78572d2e-2d2e-7857-2e2d-57782e2d5778",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "toolTip": "Tool Tip value",
  "isEndpointProtectionEnabled": true,
  "isDefault": true,
  "applicationMode": "String",
  "labelActions": [
    {
      "@odata.type": "microsoft.graph.encryptWithUserDefinedRights",
      "encryptWith": "String",
      "decryptionRightsManagementTemplateId": "Decryption Rights Management Template Id value",
      "allowMailForwarding": true,
      "allowAdHocPermissions": true
    }
  ],
  "assignedPolicies": [
    {
      "@odata.type": "microsoft.graph.labelPolicy",
      "id": "Id value"
    }
  ],
  "priority": 8,
  "autoLabeling": {
    "@odata.type": "microsoft.graph.autoLabeling",
    "sensitiveTypeIds": [
      "Sensitive Type Ids value"
    ],
    "message": "Message value"
  },
  "applicableTo": "String"
}
```

