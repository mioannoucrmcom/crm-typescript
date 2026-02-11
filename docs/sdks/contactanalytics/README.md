# ContactAnalytics

## Overview

Contact Analytics

### Available Operations

* [comCrmContactSelfServiceAnalyticsResourceGetAnalytics](#comcrmcontactselfserviceanalyticsresourcegetanalytics) - Get Contact Analytics

## comCrmContactSelfServiceAnalyticsResourceGetAnalytics

Retrieves Contact’s analytics

### Example Usage: Awards Per Month

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Awards Per Month" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "AWARDS_PER_MONTH",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "AWARDS_PER_MONTH",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Last month

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Last month" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "LAST_MONTH",
    metrics: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "LAST_MONTH",
    metrics: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Last quarter

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Last quarter" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "LAST_QUARTER",
    metrics: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "LAST_QUARTER",
    metrics: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Last six months

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Last six months" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "LAST_SIX_MONTHS",
    metrics: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "LAST_SIX_MONTHS",
    metrics: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Order Totals

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Order Totals" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "ORDER_TOTALS",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "ORDER_TOTALS",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Redeems Per Month

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Redeems Per Month" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "REDEEMS_PER_MONTH",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "REDEEMS_PER_MONTH",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: This month

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="This month" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "THIS_MONTH",
    metrics: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "THIS_MONTH",
    metrics: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```
### Example Usage: Wallet Totals

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceAnalyticsResource_getAnalytics" method="get" path="/self-service/v2/contacts/{id}/analytics" example="Wallet Totals" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactAnalytics.comCrmContactSelfServiceAnalyticsResourceGetAnalytics({
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "WALLET_TOTALS",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics } from "crm/funcs/contact-analytics-com-crm-contact-self-service-analytics-resource-get-analytics.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics(crm, {
    id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
    frequency: "<value>",
    metrics: "WALLET_TOTALS",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactAnalyticsComCrmContactSelfServiceAnalyticsResourceGetAnalytics failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsRequest](../../models/operations/com-crm-contact-self-service-analytics-resource-get-analytics-request.md)    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsResponse](../../models/operations/com-crm-contact-self-service-analytics-resource-get-analytics-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |