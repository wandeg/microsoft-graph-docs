---
title: "Update sensitivityLabel"
description: "Update the properties of a sensitivityLabel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sensitivityLabel

Update the properties of a [sensitivityLabel](../resources/sensitivitylabel.md) object.

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
PATCH /dataClassification/sensitivityLabels/{sensitivityLabelId}
PATCH /informationProtection/sensitivityLabels/{sensitivityLabelId}
PATCH /dataClassification/sensitivityLabels/{sensitivityLabelId}/sublabels/{sensitivityLabelId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [sensitivityLabel](../resources/sensitivityLabel.md) object.

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
|labelActions|[labelActionBase](../resources/labelActionBase.md) collection||
|assignedPolicies|[labelPolicy](../resources/labelPolicy.md) collection||
|priority|Int32||
|autoLabeling|[autoLabeling](../resources/autoLabeling.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [sensitivityLabel](../resources/sensitivitylabel.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sensitivitylabel"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/dataClassification/sensitivityLabels/{sensitivityLabelId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 970

{
  "@odata.type": "#microsoft.graph.sensitivityLabel",
  "id": "0f094177-4177-0f09-7741-090f7741090f",
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

