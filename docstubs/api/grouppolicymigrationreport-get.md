---
title: "Get groupPolicyMigrationReport"
description: "Read properties and relationships of the groupPolicyMigrationReport object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupPolicyMigrationReport

Namespace: microsoft.graph

Read properties and relationships of the [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object.

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
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
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
If successful, this method returns a `200 OK` response code and [groupPolicyMigrationReport](../resources/grouppolicymigrationreport.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_grouppolicymigrationreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupPolicyMigrationReport"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 762

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
    "id": "a66780eb-80eb-a667-eb80-67a6eb8067a6",
    "groupPolicyObjectId": "bfd0eb73-eb73-bfd0-73eb-d0bf73ebd0bf",
    "displayName": "Display Name value",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "groupPolicyCreatedDateTime": "2016-12-31T23:57:22.4413239+00:00",
    "groupPolicyLastModifiedDateTime": "2016-12-31T23:56:47.7454313+00:00",
    "migrationReadiness": "String",
    "targetedInActiveDirectory": true,
    "totalSettingsCount": 2,
    "supportedSettingsCount": 6,
    "supportedSettingsPercent": 8
  }
}
```

