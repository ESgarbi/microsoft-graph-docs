---
title: "Get referenceAttachment"
description: "Read the properties and relationships of a referenceAttachment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get referenceAttachment
Namespace: microsoft.graph

Read the properties and relationships of a [referenceAttachment](../resources/referenceattachment.md) object.

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
GET /referenceAttachment
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

If successful, this method returns a `200 OK` response code and a [referenceAttachment](../resources/referenceattachment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_referenceattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/referenceAttachment
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "52a9340a-340a-52a9-0a34-a9520a34a952",
    "lastModifiedDateTime": "String (timestamp)",
    "name": "String",
    "contentType": "String",
    "size": "Integer",
    "isInline": "Boolean",
    "sourceUrl": "String",
    "providerType": "String",
    "thumbnailUrl": "String",
    "previewUrl": "String",
    "permission": "String",
    "isFolder": "Boolean"
  }
}
```

