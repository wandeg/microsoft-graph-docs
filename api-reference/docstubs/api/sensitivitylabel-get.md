---
title: "Get sensitivityLabel"
description: "Read the properties and relationships of a sensitivityLabel object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get sensitivityLabel

Namespace: microsoft.graph

Read the properties and relationships of a [sensitivityLabel](../resources/sensitivitylabel.md) object.

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
GET /dataClassification/sensitivityLabels/{sensitivityLabelId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [sensitivityLabel](../resources/sensitivitylabel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sensitivitylabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitivityLabels/{sensitivityLabelId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivityLabel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

