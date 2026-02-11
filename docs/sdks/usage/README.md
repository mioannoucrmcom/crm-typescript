# Usage

## Overview

Usage

### Available Operations

* [comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords](#comcrmusagedetailrecordselfserviceresourcelistusagedetailrecords) - List Usage Records
* [comCrmUsageDetailRecordSelfServiceResourceGetMetrics](#comcrmusagedetailrecordselfserviceresourcegetmetrics) - Get Usage Records Metrics
* [comCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance](#comcrmestimateallowanceselfserviceresourceestimatesallowance) - Authorise Usage Consumption

## comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords

Retuns a list of Usage Records. Filters can be used to retrieve usage records of a specific contact or service or subscription.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.UsageDetailRecordSelfServiceResource_listUsageDetailRecords" method="get" path="/self-service/v2/contacts/{id}/usage_records" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords({
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gt]",
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
import { usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords } from "crmcom/funcs/usage-com-crm-usage-detail-record-self-service-resource-list-usage-detail-records.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords(crmcom, {
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gt]",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.UsageDetailRecordSelfServiceResource_listUsageDetailRecords" method="get" path="/self-service/v2/contacts/{id}/usage_records" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords({
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gt]",
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
import { usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords } from "crmcom/funcs/usage-com-crm-usage-detail-record-self-service-resource-list-usage-detail-records.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords(crmcom, {
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gt]",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.UsageDetailRecordSelfServiceResource_listUsageDetailRecords" method="get" path="/self-service/v2/contacts/{id}/usage_records" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords({
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gt]",
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
import { usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords } from "crmcom/funcs/usage-com-crm-usage-detail-record-self-service-resource-list-usage-detail-records.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords(crmcom, {
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gt]",
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.UsageDetailRecordSelfServiceResource_listUsageDetailRecords" method="get" path="/self-service/v2/contacts/{id}/usage_records" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords({
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gte]",
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
import { usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords } from "crmcom/funcs/usage-com-crm-usage-detail-record-self-service-resource-list-usage-detail-records.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords(crmcom, {
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[gte]",
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.UsageDetailRecordSelfServiceResource_listUsageDetailRecords" method="get" path="/self-service/v2/contacts/{id}/usage_records" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords({
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[lt]",
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
import { usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords } from "crmcom/funcs/usage-com-crm-usage-detail-record-self-service-resource-list-usage-detail-records.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords(crmcom, {
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
    usageTimestamp: "usage_timestamp[lt]",
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecords failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                            | Type                                                                                                                                                                                                 | Required                                                                                                                                                                                             | Description                                                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                            | [operations.ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsRequest](../../models/operations/com-crm-usage-detail-record-self-service-resource-list-usage-detail-records-request.md) | :heavy_check_mark:                                                                                                                                                                                   | The request object to use for the request.                                                                                                                                                           |
| `options`                                                                                                                                                                                            | RequestOptions                                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                   | Used to set various options for making HTTP requests.                                                                                                                                                |
| `options.fetchOptions`                                                                                                                                                                               | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                   | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                       |
| `options.retries`                                                                                                                                                                                    | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                   | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                     |

### Response

**Promise\<[operations.ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsResponse](../../models/operations/com-crm-usage-detail-record-self-service-resource-list-usage-detail-records-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmUsageDetailRecordSelfServiceResourceGetMetrics

Retrieve some metrics related to the usage records

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.UsageDetailRecordSelfServiceResource_getMetrics" method="get" path="/self-service/v2/contacts/{id}/usage_records/metrics" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmUsageDetailRecordSelfServiceResourceGetMetrics({
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { usageComCrmUsageDetailRecordSelfServiceResourceGetMetrics } from "crmcom/funcs/usage-com-crm-usage-detail-record-self-service-resource-get-metrics.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmUsageDetailRecordSelfServiceResourceGetMetrics(crmcom, {
    id: "13cc9948-3560-e10a-e1e4-a73610054933",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmUsageDetailRecordSelfServiceResourceGetMetrics failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmUsageDetailRecordSelfServiceResourceGetMetricsRequest](../../models/operations/com-crm-usage-detail-record-self-service-resource-get-metrics-request.md)     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmUsageDetailRecordSelfServiceResourceGetMetricsResponse](../../models/operations/com-crm-usage-detail-record-self-service-resource-get-metrics-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance

Returns an estimation on whether usage consumption is authoised or not based on purchased services allowance and how much was consumed. Web API also returns remaining allownace per service

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.EstimateAllowanceSelfServiceResource_estimatesAllowance" method="post" path="/self-service/v2/estimates/allowance" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.usage.comCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance({
    contactId: "ba48e7d3-d00a-0d28-4f9f-02b1a5b226bc",
    organisationId: "2f2a7993-6bbb-bd77-cbc8-8a2a774ef4f2",
    currencyCode: "EUR",
    service: {
      id: "<id>",
      classification: "EXPENSES_SERVICE",
    },
    blockUsage: false,
    estimationId: "271671a0-4bb3-9c2e-a9c7-6490dbfe5939",
    usage: [
      {
        product: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          sku: "FREDESPR001",
        },
      },
    ],
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { usageComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance } from "crmcom/funcs/usage-com-crm-estimate-allowance-self-service-resource-estimates-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await usageComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance(crmcom, {
    contactId: "ba48e7d3-d00a-0d28-4f9f-02b1a5b226bc",
    organisationId: "2f2a7993-6bbb-bd77-cbc8-8a2a774ef4f2",
    currencyCode: "EUR",
    service: {
      id: "<id>",
      classification: "EXPENSES_SERVICE",
    },
    blockUsage: false,
    estimationId: "271671a0-4bb3-9c2e-a9c7-6490dbfe5939",
    usage: [
      {
        product: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          sku: "FREDESPR001",
        },
      },
    ],
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("usageComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                 | Type                                                                                                                                                                                      | Required                                                                                                                                                                                  | Description                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                 | [operations.ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceRequest](../../models/operations/com-crm-estimate-allowance-self-service-resource-estimates-allowance-request.md) | :heavy_check_mark:                                                                                                                                                                        | The request object to use for the request.                                                                                                                                                |
| `options`                                                                                                                                                                                 | RequestOptions                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                        | Used to set various options for making HTTP requests.                                                                                                                                     |
| `options.fetchOptions`                                                                                                                                                                    | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                   | :heavy_minus_sign:                                                                                                                                                                        | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.            |
| `options.retries`                                                                                                                                                                         | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                        | Enables retrying HTTP requests under certain failure conditions.                                                                                                                          |

### Response

**Promise\<[operations.ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceResponse](../../models/operations/com-crm-estimate-allowance-self-service-resource-estimates-allowance-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |