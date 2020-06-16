---
title: "List singleValueLegacyExtendedProperties"
description: "Get a list of the singleValueLegacyExtendedProperty objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List singleValueLegacyExtendedProperties
Namespace: microsoft.graph

Get a list of the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects and their properties.

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
GET /users/{usersId}/messages/{messageId}/singleValueExtendedProperties
GET /users/{usersId}/contacts/{contactId}/singleValueExtendedProperties
GET /users/{usersId}/messages/{messageId}/event/singleValueExtendedProperties
GET /users/{usersId}/mailFolders/{mailFolderId}/singleValueExtendedProperties
GET /users/{usersId}/contactFolders/{contactFolderId}/singleValueExtendedProperties
GET /users/{usersId}/messages/{messageId}/event/calendar/singleValueExtendedProperties
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/singleValueExtendedProperties
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/singleValueExtendedProperties
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/singleValueExtendedProperties
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

If successful, this method returns a `200 OK` response code and a collection of [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/messages/{messageId}/singleValueExtendedProperties
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.singlevaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
      "id": "12eca0f7-a0f7-12ec-f7a0-ec12f7a0ec12",
      "value": "String"
    }
  ]
}
```

