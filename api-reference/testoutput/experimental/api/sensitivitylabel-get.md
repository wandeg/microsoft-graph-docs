---
title: "Get sensitivityLabel"
description: "Read properties and relationships of the sensitivityLabel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sensitivityLabel

Namespace: microsoft.graph

Read properties and relationships of the [sensitivityLabel](../resources/sensitivitylabel.md) object.

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
GET /dataClassification/sensitivityLabels/{sensitivityLabelId}
GET /informationProtection/sensitivityLabels/{sensitivityLabelId}
GET /dataClassification/sensitivityLabels/{sensitivityLabelId}/sublabels/{sensitivityLabelId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [sensitivityLabel](../resources/sensitivitylabel.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sensitivitylabel"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/sensitivityLabels/{sensitivityLabelId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivityLabel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

{
  "value": {
    "@odata.type": "#microsoft.graph.sensitivityLabel",
    "id": "bff54c93-4c93-bff5-934c-f5bf934cf5bf",
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
}
```

