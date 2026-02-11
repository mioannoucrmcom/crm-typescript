# Tags

## Overview

Tags

### Available Operations

* [comCrmOrganisationTagSelfServiceResourceListOrganisationTags](#comcrmorganisationtagselfserviceresourcelistorganisationtags) - List Organisation Tags
* [comCrmTagSelfServiceResourceListTags](#comcrmtagselfserviceresourcelisttags) - List Tags

## comCrmOrganisationTagSelfServiceResourceListOrganisationTags

Search through all organisation tags

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrganisationTagSelfServiceResource_listOrganisationTags" method="get" path="/self-service/v2/organisations/tags" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.tags.comCrmOrganisationTagSelfServiceResourceListOrganisationTags();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { tagsComCrmOrganisationTagSelfServiceResourceListOrganisationTags } from "crmcom/funcs/tags-com-crm-organisation-tag-self-service-resource-list-organisation-tags.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await tagsComCrmOrganisationTagSelfServiceResourceListOrganisationTags(crmcom);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tagsComCrmOrganisationTagSelfServiceResourceListOrganisationTags failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                  | Type                                                                                                                                                                                       | Required                                                                                                                                                                                   | Description                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                                  | [operations.ComCrmOrganisationTagSelfServiceResourceListOrganisationTagsRequest](../../models/operations/com-crm-organisation-tag-self-service-resource-list-organisation-tags-request.md) | :heavy_check_mark:                                                                                                                                                                         | The request object to use for the request.                                                                                                                                                 |
| `options`                                                                                                                                                                                  | RequestOptions                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                         | Used to set various options for making HTTP requests.                                                                                                                                      |
| `options.fetchOptions`                                                                                                                                                                     | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                    | :heavy_minus_sign:                                                                                                                                                                         | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.             |
| `options.retries`                                                                                                                                                                          | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                         | Enables retrying HTTP requests under certain failure conditions.                                                                                                                           |

### Response

**Promise\<[operations.ComCrmOrganisationTagSelfServiceResourceListOrganisationTagsResponse](../../models/operations/com-crm-organisation-tag-self-service-resource-list-organisation-tags-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmTagSelfServiceResourceListTags

Retrieve a list of tags based on search criteria (e.g. all contact tags)

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.TagSelfServiceResource_listTags" method="get" path="/self-service/v2/tags" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.tags.comCrmTagSelfServiceResourceListTags({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "CONTACTS",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { tagsComCrmTagSelfServiceResourceListTags } from "crmcom/funcs/tags-com-crm-tag-self-service-resource-list-tags.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await tagsComCrmTagSelfServiceResourceListTags(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "CONTACTS",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tagsComCrmTagSelfServiceResourceListTags failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.TagSelfServiceResource_listTags" method="get" path="/self-service/v2/tags" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.tags.comCrmTagSelfServiceResourceListTags({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "LEADS",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { tagsComCrmTagSelfServiceResourceListTags } from "crmcom/funcs/tags-com-crm-tag-self-service-resource-list-tags.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await tagsComCrmTagSelfServiceResourceListTags(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "LEADS",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tagsComCrmTagSelfServiceResourceListTags failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.TagSelfServiceResource_listTags" method="get" path="/self-service/v2/tags" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.tags.comCrmTagSelfServiceResourceListTags({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "ORGANISATIONS",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { tagsComCrmTagSelfServiceResourceListTags } from "crmcom/funcs/tags-com-crm-tag-self-service-resource-list-tags.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await tagsComCrmTagSelfServiceResourceListTags(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "ORGANISATIONS",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tagsComCrmTagSelfServiceResourceListTags failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.TagSelfServiceResource_listTags" method="get" path="/self-service/v2/tags" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.tags.comCrmTagSelfServiceResourceListTags({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "PRODUCTS",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { tagsComCrmTagSelfServiceResourceListTags } from "crmcom/funcs/tags-com-crm-tag-self-service-resource-list-tags.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await tagsComCrmTagSelfServiceResourceListTags(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "PRODUCTS",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tagsComCrmTagSelfServiceResourceListTags failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.TagSelfServiceResource_listTags" method="get" path="/self-service/v2/tags" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.tags.comCrmTagSelfServiceResourceListTags({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "ORGANISATIONS",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { tagsComCrmTagSelfServiceResourceListTags } from "crmcom/funcs/tags-com-crm-tag-self-service-resource-list-tags.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await tagsComCrmTagSelfServiceResourceListTags(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    entity: "ORGANISATIONS",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tagsComCrmTagSelfServiceResourceListTags failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmTagSelfServiceResourceListTagsRequest](../../models/operations/com-crm-tag-self-service-resource-list-tags-request.md)                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmTagSelfServiceResourceListTagsSecurity](../../models/operations/com-crm-tag-self-service-resource-list-tags-security.md)                                     | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmTagSelfServiceResourceListTagsResponse](../../models/operations/com-crm-tag-self-service-resource-list-tags-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |