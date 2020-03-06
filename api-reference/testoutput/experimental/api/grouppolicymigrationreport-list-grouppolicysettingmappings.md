---
title: "List groupPolicySettingMappings"
description: "Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupPolicySettingMappings

Namespace: microsoft.graph

Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property.

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
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
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
If successful, this method returns a `200 OK` response code and a collection of [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouppolicysettingmapping"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicysettingmapping)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1062

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
      "id": "17f8a4a9-a4a9-17f8-a9a4-f817a9a4f817",
      "parentId": "Parent Id value",
      "childIdList": [
        "Child Id List value"
      ],
      "settingName": "Setting Name value",
      "settingValue": "Setting Value value",
      "settingValueType": "Setting Value Type value",
      "settingDisplayName": "Setting Display Name value",
      "settingDisplayValue": "Setting Display Value value",
      "settingDisplayValueType": "Setting Display Value Type value",
      "settingValueDisplayUnits": "Setting Value Display Units value",
      "settingCategory": "Setting Category value",
      "mdmCspName": "Mdm Csp Name value",
      "mdmSettingUri": "Mdm Setting Uri value",
      "mdmMinimumOSVersion": 3,
      "settingType": "String",
      "isMdmSupported": true,
      "mdmSupportedState": "String",
      "settingScope": "String",
      "intuneSettingUriList": [
        "Intune Setting Uri List value"
      ]
    }
  ]
}
```

