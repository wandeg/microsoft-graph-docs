---
title: "Get eventMessageRequest"
description: "Read properties and relationships of the eventMessageRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get eventMessageRequest

Read properties and relationships of the [eventMessageRequest](../resources/eventmessagerequest.md) object.

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
GET ** Entity URI for microsoft.graph.eventMessageRequest not found
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
If successful, this method returns a `200 OK` response code and [eventMessageRequest](../resources/eventmessagerequest.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_eventmessagerequest"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.eventMessageRequest not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5058

{
  "value": {
    "@odata.type": "#microsoft.graph.eventMessageRequest",
    "id": "083b94ba-94ba-083b-ba94-3b08ba943b08",
    "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "receivedDateTime": "2016-12-31T23:59:48.3455349+03:00",
    "sentDateTime": "2016-12-31T23:58:59.7348131+03:00",
    "hasAttachments": true,
    "internetMessageId": "Internet Message Id value",
    "internetMessageHeaders": [
      {
        "@odata.type": "microsoft.graph.internetMessageHeader",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "subject": "Subject value",
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "bodyPreview": "Body Preview value",
    "importance": "String",
    "parentFolderId": "Parent Folder Id value",
    "sender": {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "address": "Address value"
      }
    },
    "from": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "toRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "bccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "replyTo": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "Conversation Id value",
    "conversationIndex": "Y29udmVyc2F0aW9uSW5kZXg=",
    "uniqueBody": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "isDeliveryReceiptRequested": true,
    "isReadReceiptRequested": true,
    "isRead": true,
    "isDraft": true,
    "webLink": "Web Link value",
    "mentionsPreview": {
      "@odata.type": "microsoft.graph.mentionsPreview",
      "isMentioned": true
    },
    "inferenceClassification": "String",
    "unsubscribeData": [
      "Unsubscribe Data value"
    ],
    "unsubscribeEnabled": true,
    "flag": {
      "@odata.type": "microsoft.graph.followupFlag",
      "completedDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone",
        "dateTime": "Date Time value",
        "timeZone": "Time Zone value"
      },
      "dueDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "startDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "flagStatus": "String"
    },
    "meetingMessageType": "String",
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "endDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "location": {
      "@odata.type": "microsoft.graph.location",
      "displayName": "Display Name value",
      "locationEmailAddress": "Location Email Address value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "type": "String",
        "postOfficeBox": "Post Office Box value",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "coordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "altitude": "Double",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitudeAccuracy": "Double"
      },
      "locationUri": "Location Uri value",
      "locationType": "String",
      "uniqueId": "Unique Id value",
      "uniqueIdType": "String"
    },
    "type": "String",
    "recurrence": {
      "@odata.type": "microsoft.graph.patternedRecurrence",
      "pattern": {
        "@odata.type": "microsoft.graph.recurrencePattern",
        "type": "String",
        "interval": 8,
        "month": 5,
        "dayOfMonth": 10,
        "daysOfWeek": [
          "String"
        ],
        "firstDayOfWeek": "String",
        "index": "String"
      },
      "range": {
        "@odata.type": "microsoft.graph.recurrenceRange",
        "type": "String",
        "startDate": "Date",
        "endDate": "Date",
        "recurrenceTimeZone": "Recurrence Time Zone value",
        "numberOfOccurrences": 3
      }
    },
    "isOutOfDate": true,
    "isAllDay": true,
    "isDelegated": true,
    "previousLocation": {
      "@odata.type": "microsoft.graph.location"
    },
    "previousStartDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "previousEndDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "responseRequested": true,
    "allowNewTimeProposals": true
  }
}
```

