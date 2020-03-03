---
title: "Get alert"
description: "Read properties and relationships of the alert object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get alert

Read properties and relationships of the [alert](../resources/alert.md) object.

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
GET /Security/alerts/{alertId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [alert](../resources/alert.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_alert"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/Security/alerts/{alertId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5736

{
  "value": {
    "@odata.type": "#microsoft.graph.alert",
    "id": "0d568ad6-8ad6-0d56-d68a-560dd68a560d",
    "activityGroupName": "Activity Group Name value",
    "assignedTo": "Assigned To value",
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureTenantId": "Azure Tenant Id value",
    "category": "Category value",
    "closedDateTime": "2017-01-01T00:02:18.6868486+03:00",
    "cloudAppStates": [
      {
        "@odata.type": "microsoft.graph.cloudAppSecurityState",
        "destinationServiceIp": "Destination Service Ip value",
        "destinationServiceName": "Destination Service Name value",
        "riskScore": "Risk Score value"
      }
    ],
    "comments": [
      "Comments value"
    ],
    "confidence": 10,
    "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
    "description": "Description value",
    "detectionIds": [
      "Detection Ids value"
    ],
    "eventDateTime": "2017-01-01T00:01:33.1647467+03:00",
    "feedback": "String",
    "fileStates": [
      {
        "@odata.type": "microsoft.graph.fileSecurityState",
        "fileHash": {
          "@odata.type": "microsoft.graph.fileHash",
          "hashType": "String",
          "hashValue": "Hash Value value"
        },
        "name": "Name value",
        "path": "Path value"
      }
    ],
    "historyStates": [
      {
        "@odata.type": "microsoft.graph.alertHistoryState",
        "appId": "App Id value",
        "status": "String",
        "updatedDateTime": "2017-01-01T00:02:39.6439205+03:00",
        "user": "User value"
      }
    ],
    "hostStates": [
      {
        "@odata.type": "microsoft.graph.hostSecurityState",
        "fqdn": "Fqdn value",
        "isAzureAdJoined": true,
        "isAzureAdRegistered": true,
        "isHybridAzureDomainJoined": true,
        "netBiosName": "Net Bios Name value",
        "os": "Os value",
        "privateIpAddress": "Private Ip Address value",
        "publicIpAddress": "Public Ip Address value"
      }
    ],
    "lastModifiedDateTime": "2016-12-31T23:59:09.8413999+03:00",
    "malwareStates": [
      {
        "@odata.type": "microsoft.graph.malwareState",
        "family": "Family value",
        "severity": "Severity value",
        "wasRunning": true
      }
    ],
    "networkConnections": [
      {
        "@odata.type": "microsoft.graph.networkConnection",
        "applicationName": "Application Name value",
        "destinationAddress": "Destination Address value",
        "destinationDomain": "Destination Domain value",
        "destinationPort": "Destination Port value",
        "destinationUrl": "https://example.com/destinationUrl/",
        "direction": "String",
        "domainRegisteredDateTime": "2016-12-31T23:57:40.0212945+03:00",
        "localDnsName": "Local Dns Name value",
        "natDestinationAddress": "Nat Destination Address value",
        "natDestinationPort": "Nat Destination Port value",
        "natSourceAddress": "Nat Source Address value",
        "natSourcePort": "Nat Source Port value",
        "protocol": "String",
        "sourceAddress": "Source Address value",
        "sourcePort": "Source Port value",
        "status": "String",
        "urlParameters": "Url Parameters value"
      }
    ],
    "processes": [
      {
        "@odata.type": "microsoft.graph.process",
        "accountName": "Account Name value",
        "commandLine": "Command Line value",
        "integrityLevel": "String",
        "isElevated": true,
        "parentProcessCreatedDateTime": "2016-12-31T23:58:20.1943249+03:00",
        "parentProcessId": 15,
        "parentProcessName": "Parent Process Name value",
        "processId": 9
      }
    ],
    "recommendedActions": [
      "Recommended Actions value"
    ],
    "registryKeyStates": [
      {
        "@odata.type": "microsoft.graph.registryKeyState",
        "hive": "String",
        "key": "Key value",
        "oldKey": "Old Key value",
        "oldValueData": "Old Value Data value",
        "oldValueName": "Old Value Name value",
        "operation": "String",
        "valueData": "Value Data value",
        "valueName": "Value Name value",
        "valueType": "String"
      }
    ],
    "severity": "String",
    "sourceMaterials": [
      "Source Materials value"
    ],
    "status": "String",
    "tags": [
      "Tags value"
    ],
    "title": "Title value",
    "triggers": [
      {
        "@odata.type": "microsoft.graph.alertTrigger",
        "type": "Type value",
        "value": "Value value"
      }
    ],
    "userStates": [
      {
        "@odata.type": "microsoft.graph.userSecurityState",
        "aadUserId": "Aad User Id value",
        "domainName": "Domain Name value",
        "emailRole": "String",
        "isVpn": true,
        "logonDateTime": "2017-01-01T00:02:19.4310282+03:00",
        "logonId": "Logon Id value",
        "logonIp": "Logon Ip value",
        "logonLocation": "Logon Location value",
        "logonType": "String",
        "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
        "userAccountType": "String",
        "userPrincipalName": "User Principal Name value"
      }
    ],
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation",
      "provider": "Provider value",
      "providerVersion": "Provider Version value",
      "subProvider": "Sub Provider value",
      "vendor": "Vendor value"
    },
    "vulnerabilityStates": [
      {
        "@odata.type": "microsoft.graph.vulnerabilityState",
        "cve": "Cve value"
      }
    ]
  }
}
```

