---
title: "List groupPolicySettingMappings"
description: "Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List groupPolicySettingMappings

Namespace: microsoft.graph

Get the groupPolicySettingMappings from the groupPolicySettingMappings navigation property.

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
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_grouppolicysettingmapping"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouppolicysettingmapping)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
      "id": "80962cfe-2cfe-8096-fe2c-9680fe2c9680",
      "parentId": "String",
      "childIdList": [
        "String"
      ],
      "settingName": "String",
      "settingValue": "String",
      "settingValueType": "String",
      "settingDisplayName": "String",
      "settingDisplayValue": "String",
      "settingDisplayValueType": "String",
      "settingValueDisplayUnits": "String",
      "settingCategory": "String",
      "mdmCspName": "String",
      "mdmSettingUri": "String",
      "mdmMinimumOSVersion": "Integer",
      "settingType": "String",
      "isMdmSupported": "Boolean",
      "mdmSupportedState": "String",
      "settingScope": "String",
      "intuneSettingUriList": [
        "String"
      ],
      "intuneSettingDefinitionId": "String"
    }
  ]
}
```

