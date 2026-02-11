# Passes

## Overview

Passes

### Available Operations

* [comCrmPassPlanSelfServiceResourceListPassTypes](#comcrmpassplanselfserviceresourcelistpasstypes) - List Pass Plans
* [comCrmPassSelfServiceResourceRedeemPass](#comcrmpassselfserviceresourceredeempass) - Redeem Pass
* [comCrmPassSelfServiceResourceViewPromoPass](#comcrmpassselfserviceresourceviewpromopass) - View promo pass

## comCrmPassPlanSelfServiceResourceListPassTypes

Retrieve all pass plans with GIFT classifcation that issue electronic passes. Only active pass plans that are related with a product will be acquired.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PassPlanSelfServiceResource_listPassTypes" method="get" path="/self-service/v2/pass_plans" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.passes.comCrmPassPlanSelfServiceResourceListPassTypes({
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
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
import { passesComCrmPassPlanSelfServiceResourceListPassTypes } from "crmcom/funcs/passes-com-crm-pass-plan-self-service-resource-list-pass-types.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassPlanSelfServiceResourceListPassTypes(crmcom, {
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("passesComCrmPassPlanSelfServiceResourceListPassTypes failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.PassPlanSelfServiceResource_listPassTypes" method="get" path="/self-service/v2/pass_plans" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.passes.comCrmPassPlanSelfServiceResourceListPassTypes({
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
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
import { passesComCrmPassPlanSelfServiceResourceListPassTypes } from "crmcom/funcs/passes-com-crm-pass-plan-self-service-resource-list-pass-types.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassPlanSelfServiceResourceListPassTypes(crmcom, {
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("passesComCrmPassPlanSelfServiceResourceListPassTypes failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.PassPlanSelfServiceResource_listPassTypes" method="get" path="/self-service/v2/pass_plans" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.passes.comCrmPassPlanSelfServiceResourceListPassTypes({
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
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
import { passesComCrmPassPlanSelfServiceResourceListPassTypes } from "crmcom/funcs/passes-com-crm-pass-plan-self-service-resource-list-pass-types.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassPlanSelfServiceResourceListPassTypes(crmcom, {
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("passesComCrmPassPlanSelfServiceResourceListPassTypes failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PassPlanSelfServiceResource_listPassTypes" method="get" path="/self-service/v2/pass_plans" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.passes.comCrmPassPlanSelfServiceResourceListPassTypes({
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
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
import { passesComCrmPassPlanSelfServiceResourceListPassTypes } from "crmcom/funcs/passes-com-crm-pass-plan-self-service-resource-list-pass-types.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassPlanSelfServiceResourceListPassTypes(crmcom, {
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("passesComCrmPassPlanSelfServiceResourceListPassTypes failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PassPlanSelfServiceResource_listPassTypes" method="get" path="/self-service/v2/pass_plans" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.passes.comCrmPassPlanSelfServiceResourceListPassTypes({
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
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
import { passesComCrmPassPlanSelfServiceResourceListPassTypes } from "crmcom/funcs/passes-com-crm-pass-plan-self-service-resource-list-pass-types.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassPlanSelfServiceResourceListPassTypes(crmcom, {
    currencyCode: "\"EUR\"",
    productId: "99869C84FA60F9FE407140E20F707726",
    searchValue: "Xmas Plans",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("passesComCrmPassPlanSelfServiceResourceListPassTypes failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPassPlanSelfServiceResourceListPassTypesRequest](../../models/operations/com-crm-pass-plan-self-service-resource-list-pass-types-request.md)                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPassPlanSelfServiceResourceListPassTypesResponse](../../models/operations/com-crm-pass-plan-self-service-resource-list-pass-types-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPassSelfServiceResourceRedeemPass

Redeems a single pass by a contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PassSelfServiceResource_redeemPass" method="post" path="/self-service/v2/passes/redeem" example="Redeem Pass" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.passes.comCrmPassSelfServiceResourceRedeemPass({
    code: "CRM59934377COM",
    contactId: "00dc6a3d-2c90-4953-b1db-92c81d004406",
    walletId: "228568ea-ab6f-471e-bae7-7adb7e913ff6",
    pin: "0103",
    organisation: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      merchantTap: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        code: "2131424123",
      },
      venueTap: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        code: "2131424123",
      },
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { passesComCrmPassSelfServiceResourceRedeemPass } from "crmcom/funcs/passes-com-crm-pass-self-service-resource-redeem-pass.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassSelfServiceResourceRedeemPass(crmcom, {
    code: "CRM59934377COM",
    contactId: "00dc6a3d-2c90-4953-b1db-92c81d004406",
    walletId: "228568ea-ab6f-471e-bae7-7adb7e913ff6",
    pin: "0103",
    organisation: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      merchantTap: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        code: "2131424123",
      },
      venueTap: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        code: "2131424123",
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("passesComCrmPassSelfServiceResourceRedeemPass failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPassSelfServiceResourceRedeemPassRequest](../../models/operations/com-crm-pass-self-service-resource-redeem-pass-request.md)                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPassSelfServiceResourceRedeemPassResponse](../../models/operations/com-crm-pass-self-service-resource-redeem-pass-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPassSelfServiceResourceViewPromoPass

View promo pass - An HTML based landing page is returned and rendered

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PassSelfServiceResource_viewPromoPass" method="get" path="/self-service/v2/passes/view_promo_pass" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.passes.comCrmPassSelfServiceResourceViewPromoPass();


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { passesComCrmPassSelfServiceResourceViewPromoPass } from "crmcom/funcs/passes-com-crm-pass-self-service-resource-view-promo-pass.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await passesComCrmPassSelfServiceResourceViewPromoPass(crmcom);
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("passesComCrmPassSelfServiceResourceViewPromoPass failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPassSelfServiceResourceViewPromoPassRequest](../../models/operations/com-crm-pass-self-service-resource-view-promo-pass-request.md)                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |