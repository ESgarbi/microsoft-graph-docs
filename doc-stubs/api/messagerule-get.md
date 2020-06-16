---
title: "Get messageRule"
description: "Read the properties and relationships of a messageRule object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get messageRule
Namespace: microsoft.graph

Read the properties and relationships of a [messageRule](../resources/messagerule.md) object.

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
GET /users/{usersId}/mailFolders/{mailFolderId}/messageRules/{messageRuleId}
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

If successful, this method returns a `200 OK` response code and a [messageRule](../resources/messagerule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mailFolders/{mailFolderId}/messageRules/{messageRuleId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.messageRule",
    "id": "7fe8c515-c515-7fe8-15c5-e87f15c5e87f",
    "displayName": "String",
    "sequence": "Integer",
    "conditions": {
      "@odata.type": "microsoft.graph.messageRulePredicates"
    },
    "actions": {
      "@odata.type": "microsoft.graph.messageRuleActions"
    },
    "exceptions": {
      "@odata.type": "microsoft.graph.messageRulePredicates"
    },
    "isEnabled": "Boolean",
    "hasError": "Boolean",
    "isReadOnly": "Boolean"
  }
}
```

