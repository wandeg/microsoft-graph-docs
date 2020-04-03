---
title: "List sensitivityLabels"
description: "Get the sensitivityLabels from the sensitivityLabels navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sensitivityLabels

Namespace: microsoft.graph

Get the sensitivityLabels from the sensitivityLabels navigation property.

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
GET /dataClassification/sensitivityLabels
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [sensitivityLabel](../resources/sensitivitylabel.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sensitivitylabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitivityLabels
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sensitivitylabel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1164

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sensitivityLabel",
      "id": "9a875d57-5d57-9a87-575d-879a575d879a",
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
  ]
}
```

