---
title: "Create sensitivityLabel"
description: "Create a new sensitivityLabel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sensitivityLabel

Namespace: microsoft.graph

Create a new [sensitivityLabel](../resources/sensitivitylabel.md) object.

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
POST /dataClassification/sensitivityLabels
POST /informationProtection/sensitivityLabels
POST /dataClassification/sensitivityLabels/{sensitivityLabelId}/sublabels
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [sensitivityLabel](../resources/sensitivitylabel.md) object.

The following table shows the properties that are required when you create the [sensitivityLabel](../resources/sensitivitylabel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|displayName|String||
|description|String||
|toolTip|String||
|isEndpointProtectionEnabled|Boolean||
|isDefault|Boolean||
|applicationMode|Enumeration|. Possible values are: `manual`, `automatic`, `recommended`.|
|labelActions|[labelActionBase](../resources/labelactionbase.md) collection||
|assignedPolicies|[labelPolicy](../resources/labelpolicy.md) collection||
|priority|Int32||
|autoLabeling|[autoLabeling](../resources/autolabeling.md)||



## Response
If successful, this method returns a `201 Created` response code and a [sensitivityLabel](../resources/sensitivitylabel.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sensitivitylabel_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/dataClassification/sensitivityLabels
Content-type: application/json
Content-length: 921

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
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivitylabel"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 970

{
  "@odata.type": "#microsoft.graph.sensitivityLabel",
  "id": "746d2913-2913-746d-1329-6d7413296d74",
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
  }
}
```

