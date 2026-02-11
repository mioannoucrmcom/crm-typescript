# Settings

## Overview

Settings

### Available Operations

* [comCrmNameDayRulesSelfServiceResourceListNameDayRules](#comcrmnamedayrulesselfserviceresourcelistnamedayrules) - List Name Day Rules
* [comCrmProductBrandSelfServiceResourceGetProductBrands](#comcrmproductbrandselfserviceresourcegetproductbrands) - List Product Brands
* [comCrmProductCategorySelfServiceResourceListProductCategories](#comcrmproductcategoryselfserviceresourcelistproductcategories) - List Product Categories
* [comCrmProductTypeSelfServiceResourceListProductTypes](#comcrmproducttypeselfserviceresourcelistproducttypes) - List Product Types

## comCrmNameDayRulesSelfServiceResourceListNameDayRules

Returns a list of name day rules

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.NameDayRulesSelfServiceResource_listNameDayRules" method="get" path="/self-service/v2/name_day_rules" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmNameDayRulesSelfServiceResourceListNameDayRules();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { settingsComCrmNameDayRulesSelfServiceResourceListNameDayRules } from "crm/funcs/settings-com-crm-name-day-rules-self-service-resource-list-name-day-rules.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmNameDayRulesSelfServiceResourceListNameDayRules(crm);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmNameDayRulesSelfServiceResourceListNameDayRules failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmNameDayRulesSelfServiceResourceListNameDayRulesRequest](../../models/operations/com-crm-name-day-rules-self-service-resource-list-name-day-rules-request.md) | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmNameDayRulesSelfServiceResourceListNameDayRulesResponse](../../models/operations/com-crm-name-day-rules-self-service-resource-list-name-day-rules-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductBrandSelfServiceResourceGetProductBrands

Returns a list of product brands

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductBrandSelfServiceResource_getProductBrands" method="get" path="/self-service/v2/products/brands" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductBrandSelfServiceResourceGetProductBrands({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductBrandSelfServiceResourceGetProductBrands } from "crm/funcs/settings-com-crm-product-brand-self-service-resource-get-product-brands.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductBrandSelfServiceResourceGetProductBrands(crm, {
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductBrandSelfServiceResourceGetProductBrands failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductBrandSelfServiceResource_getProductBrands" method="get" path="/self-service/v2/products/brands" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductBrandSelfServiceResourceGetProductBrands({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductBrandSelfServiceResourceGetProductBrands } from "crm/funcs/settings-com-crm-product-brand-self-service-resource-get-product-brands.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductBrandSelfServiceResourceGetProductBrands(crm, {
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductBrandSelfServiceResourceGetProductBrands failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductBrandSelfServiceResource_getProductBrands" method="get" path="/self-service/v2/products/brands" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductBrandSelfServiceResourceGetProductBrands({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductBrandSelfServiceResourceGetProductBrands } from "crm/funcs/settings-com-crm-product-brand-self-service-resource-get-product-brands.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductBrandSelfServiceResourceGetProductBrands(crm, {
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductBrandSelfServiceResourceGetProductBrands failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductBrandSelfServiceResource_getProductBrands" method="get" path="/self-service/v2/products/brands" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductBrandSelfServiceResourceGetProductBrands({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductBrandSelfServiceResourceGetProductBrands } from "crm/funcs/settings-com-crm-product-brand-self-service-resource-get-product-brands.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductBrandSelfServiceResourceGetProductBrands(crm, {
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductBrandSelfServiceResourceGetProductBrands failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductBrandSelfServiceResource_getProductBrands" method="get" path="/self-service/v2/products/brands" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductBrandSelfServiceResourceGetProductBrands({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductBrandSelfServiceResourceGetProductBrands } from "crm/funcs/settings-com-crm-product-brand-self-service-resource-get-product-brands.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductBrandSelfServiceResourceGetProductBrands(crm, {
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductBrandSelfServiceResourceGetProductBrands failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmProductBrandSelfServiceResourceGetProductBrandsRequest](../../models/operations/com-crm-product-brand-self-service-resource-get-product-brands-request.md)   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmProductBrandSelfServiceResourceGetProductBrandsResponse](../../models/operations/com-crm-product-brand-self-service-resource-get-product-brands-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductCategorySelfServiceResourceListProductCategories

Returns a list of product categories

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductCategorySelfServiceResource_listProductCategories" method="get" path="/self-service/v2/products/categories" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductCategorySelfServiceResourceListProductCategories({
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductCategorySelfServiceResourceListProductCategories } from "crm/funcs/settings-com-crm-product-category-self-service-resource-list-product-categories.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductCategorySelfServiceResourceListProductCategories(crm, {
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductCategorySelfServiceResourceListProductCategories failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductCategorySelfServiceResource_listProductCategories" method="get" path="/self-service/v2/products/categories" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductCategorySelfServiceResourceListProductCategories({
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductCategorySelfServiceResourceListProductCategories } from "crm/funcs/settings-com-crm-product-category-self-service-resource-list-product-categories.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductCategorySelfServiceResourceListProductCategories(crm, {
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductCategorySelfServiceResourceListProductCategories failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductCategorySelfServiceResource_listProductCategories" method="get" path="/self-service/v2/products/categories" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductCategorySelfServiceResourceListProductCategories({
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductCategorySelfServiceResourceListProductCategories } from "crm/funcs/settings-com-crm-product-category-self-service-resource-list-product-categories.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductCategorySelfServiceResourceListProductCategories(crm, {
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductCategorySelfServiceResourceListProductCategories failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductCategorySelfServiceResource_listProductCategories" method="get" path="/self-service/v2/products/categories" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductCategorySelfServiceResourceListProductCategories({
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductCategorySelfServiceResourceListProductCategories } from "crm/funcs/settings-com-crm-product-category-self-service-resource-list-product-categories.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductCategorySelfServiceResourceListProductCategories(crm, {
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductCategorySelfServiceResourceListProductCategories failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductCategorySelfServiceResource_listProductCategories" method="get" path="/self-service/v2/products/categories" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductCategorySelfServiceResourceListProductCategories({
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductCategorySelfServiceResourceListProductCategories } from "crm/funcs/settings-com-crm-product-category-self-service-resource-list-product-categories.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductCategorySelfServiceResourceListProductCategories(crm, {
    availableInOrderMenus: false,
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductCategorySelfServiceResourceListProductCategories failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                    | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                    | [operations.ComCrmProductCategorySelfServiceResourceListProductCategoriesRequest](../../models/operations/com-crm-product-category-self-service-resource-list-product-categories-request.md) | :heavy_check_mark:                                                                                                                                                                           | The request object to use for the request.                                                                                                                                                   |
| `options`                                                                                                                                                                                    | RequestOptions                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                           | Used to set various options for making HTTP requests.                                                                                                                                        |
| `options.fetchOptions`                                                                                                                                                                       | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                      | :heavy_minus_sign:                                                                                                                                                                           | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.               |
| `options.retries`                                                                                                                                                                            | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                           | Enables retrying HTTP requests under certain failure conditions.                                                                                                                             |

### Response

**Promise\<[operations.ComCrmProductCategorySelfServiceResourceListProductCategoriesResponse](../../models/operations/com-crm-product-category-self-service-resource-list-product-categories-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductTypeSelfServiceResourceListProductTypes

Returns a list of product types

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductTypeSelfServiceResource_listProductTypes" method="get" path="/self-service/v2/products/types" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductTypeSelfServiceResourceListProductTypes({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductTypeSelfServiceResourceListProductTypes } from "crm/funcs/settings-com-crm-product-type-self-service-resource-list-product-types.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductTypeSelfServiceResourceListProductTypes(crm, {
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductTypeSelfServiceResourceListProductTypes failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductTypeSelfServiceResource_listProductTypes" method="get" path="/self-service/v2/products/types" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductTypeSelfServiceResourceListProductTypes({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductTypeSelfServiceResourceListProductTypes } from "crm/funcs/settings-com-crm-product-type-self-service-resource-list-product-types.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductTypeSelfServiceResourceListProductTypes(crm, {
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductTypeSelfServiceResourceListProductTypes failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductTypeSelfServiceResource_listProductTypes" method="get" path="/self-service/v2/products/types" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductTypeSelfServiceResourceListProductTypes({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductTypeSelfServiceResourceListProductTypes } from "crm/funcs/settings-com-crm-product-type-self-service-resource-list-product-types.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductTypeSelfServiceResourceListProductTypes(crm, {
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductTypeSelfServiceResourceListProductTypes failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductTypeSelfServiceResource_listProductTypes" method="get" path="/self-service/v2/products/types" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductTypeSelfServiceResourceListProductTypes({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductTypeSelfServiceResourceListProductTypes } from "crm/funcs/settings-com-crm-product-type-self-service-resource-list-product-types.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductTypeSelfServiceResourceListProductTypes(crm, {
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductTypeSelfServiceResourceListProductTypes failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductTypeSelfServiceResource_listProductTypes" method="get" path="/self-service/v2/products/types" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.settings.comCrmProductTypeSelfServiceResourceListProductTypes({
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
import { CrmCore } from "crm/core.js";
import { settingsComCrmProductTypeSelfServiceResourceListProductTypes } from "crm/funcs/settings-com-crm-product-type-self-service-resource-list-product-types.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await settingsComCrmProductTypeSelfServiceResourceListProductTypes(crm, {
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("settingsComCrmProductTypeSelfServiceResourceListProductTypes failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmProductTypeSelfServiceResourceListProductTypesRequest](../../models/operations/com-crm-product-type-self-service-resource-list-product-types-request.md)     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmProductTypeSelfServiceResourceListProductTypesResponse](../../models/operations/com-crm-product-type-self-service-resource-list-product-types-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |