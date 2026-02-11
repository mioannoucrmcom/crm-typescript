# Promotions

## Overview

Promotions

### Available Operations

* [comCrmPromotionSelfServiceResourceList](#comcrmpromotionselfserviceresourcelist) - List Promotions
* [comCrmPromotionSelfServiceResourceGetSingle](#comcrmpromotionselfserviceresourcegetsingle) - Get Promotion

## comCrmPromotionSelfServiceResourceList

Returns a list of Promotions.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PromotionSelfServiceResource_list" method="get" path="/self-service/v2/promotions" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.promotions.comCrmPromotionSelfServiceResourceList({
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
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
import { promotionsComCrmPromotionSelfServiceResourceList } from "crmcom/funcs/promotions-com-crm-promotion-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await promotionsComCrmPromotionSelfServiceResourceList(crmcom, {
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("promotionsComCrmPromotionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.PromotionSelfServiceResource_list" method="get" path="/self-service/v2/promotions" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.promotions.comCrmPromotionSelfServiceResourceList({
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
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
import { promotionsComCrmPromotionSelfServiceResourceList } from "crmcom/funcs/promotions-com-crm-promotion-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await promotionsComCrmPromotionSelfServiceResourceList(crmcom, {
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("promotionsComCrmPromotionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.PromotionSelfServiceResource_list" method="get" path="/self-service/v2/promotions" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.promotions.comCrmPromotionSelfServiceResourceList({
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
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
import { promotionsComCrmPromotionSelfServiceResourceList } from "crmcom/funcs/promotions-com-crm-promotion-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await promotionsComCrmPromotionSelfServiceResourceList(crmcom, {
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("promotionsComCrmPromotionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PromotionSelfServiceResource_list" method="get" path="/self-service/v2/promotions" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.promotions.comCrmPromotionSelfServiceResourceList({
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
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
import { promotionsComCrmPromotionSelfServiceResourceList } from "crmcom/funcs/promotions-com-crm-promotion-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await promotionsComCrmPromotionSelfServiceResourceList(crmcom, {
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("promotionsComCrmPromotionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PromotionSelfServiceResource_list" method="get" path="/self-service/v2/promotions" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.promotions.comCrmPromotionSelfServiceResourceList({
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
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
import { promotionsComCrmPromotionSelfServiceResourceList } from "crmcom/funcs/promotions-com-crm-promotion-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await promotionsComCrmPromotionSelfServiceResourceList(crmcom, {
    organisations: "49c9554f-f1af-4d41-becf-7a2094cffd29,7223c237-f857-4140-a150-13ceef960f6e",
    searchValue: "Happy Hour",
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("promotionsComCrmPromotionSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPromotionSelfServiceResourceListRequest](../../models/operations/com-crm-promotion-self-service-resource-list-request.md)                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPromotionSelfServiceResourceListResponse](../../models/operations/com-crm-promotion-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPromotionSelfServiceResourceGetSingle

Retrieve detailed information for a specific promotion

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PromotionSelfServiceResource_getSingle" method="get" path="/self-service/v2/promotions/{id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.promotions.comCrmPromotionSelfServiceResourceGetSingle({
    id: "6eeec3be-be1b-3eae-ca11-779d932d97fc",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { promotionsComCrmPromotionSelfServiceResourceGetSingle } from "crmcom/funcs/promotions-com-crm-promotion-self-service-resource-get-single.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await promotionsComCrmPromotionSelfServiceResourceGetSingle(crmcom, {
    id: "6eeec3be-be1b-3eae-ca11-779d932d97fc",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("promotionsComCrmPromotionSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPromotionSelfServiceResourceGetSingleRequest](../../models/operations/com-crm-promotion-self-service-resource-get-single-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPromotionSelfServiceResourceGetSingleResponse](../../models/operations/com-crm-promotion-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |