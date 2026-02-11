# Recommendations

## Overview

Recommendations

### Available Operations

* [comCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation](#comcrmorderproductrecommendationselfserviceresourcegetorderproductrecommendation) - Order Product Recommendation Self-Service
* [comCrmProductRecommendationSelfServiceResourceGetProductRecommendation](#comcrmproductrecommendationselfserviceresourcegetproductrecommendation) - Product Recommendation
* [comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation](#comcrmservicerecommendationselfserviceresourcegetservicerecommendation) - Service Recommendation

## comCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation

Provide product recommendations to contacts/organisations on additional products that can be included in their Order.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderProductRecommendationSelfServiceResource_getOrderProductRecommendation" method="get" path="/self-service/v2/orders/recommendation" example="Order Product Recommendation Response" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    estimationId: "<id>",
    includeCreatives: true,
    includeCrossSells: true,
    includePromotions: true,
    includeRewardOffers: true,
    includeUpsells: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import {
  recommendationsComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation,
} from "crm/funcs/recommendations-com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    estimationId: "<id>",
    includeCreatives: true,
    includeCrossSells: true,
    includePromotions: true,
    includeRewardOffers: true,
    includeUpsells: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendation failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                                              | Type                                                                                                                                                                                                                                   | Required                                                                                                                                                                                                                               | Description                                                                                                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                                              | [operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationRequest](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-request.md)   | :heavy_check_mark:                                                                                                                                                                                                                     | The request object to use for the request.                                                                                                                                                                                             |
| `security`                                                                                                                                                                                                                             | [operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationSecurity](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-security.md) | :heavy_check_mark:                                                                                                                                                                                                                     | The security requirements to use for the request.                                                                                                                                                                                      |
| `options`                                                                                                                                                                                                                              | RequestOptions                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                     | Used to set various options for making HTTP requests.                                                                                                                                                                                  |
| `options.fetchOptions`                                                                                                                                                                                                                 | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                                                                     | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                                         |
| `options.retries`                                                                                                                                                                                                                      | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                     | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                                       |

### Response

**Promise\<[operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationResponse](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductRecommendationSelfServiceResourceGetProductRecommendation

Provide product recommendations to contacts/organisations on additional products that can be included in their Order.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductRecommendationSelfServiceResource_getProductRecommendation" method="get" path="/self-service/v2/products/recommendation" example="Product Recommendation Response" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmProductRecommendationSelfServiceResourceGetProductRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import {
  recommendationsComCrmProductRecommendationSelfServiceResourceGetProductRecommendation,
} from "crm/funcs/recommendations-com-crm-product-recommendation-self-service-resource-get-product-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmProductRecommendationSelfServiceResourceGetProductRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmProductRecommendationSelfServiceResourceGetProductRecommendation failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                        | Type                                                                                                                                                                                                             | Required                                                                                                                                                                                                         | Description                                                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                        | [operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationRequest](../../models/operations/com-crm-product-recommendation-self-service-resource-get-product-recommendation-request.md)   | :heavy_check_mark:                                                                                                                                                                                               | The request object to use for the request.                                                                                                                                                                       |
| `security`                                                                                                                                                                                                       | [operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationSecurity](../../models/operations/com-crm-product-recommendation-self-service-resource-get-product-recommendation-security.md) | :heavy_check_mark:                                                                                                                                                                                               | The security requirements to use for the request.                                                                                                                                                                |
| `options`                                                                                                                                                                                                        | RequestOptions                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                               | Used to set various options for making HTTP requests.                                                                                                                                                            |
| `options.fetchOptions`                                                                                                                                                                                           | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                               | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                   |
| `options.retries`                                                                                                                                                                                                | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                               | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                 |

### Response

**Promise\<[operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationResponse[]](../../models/.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation

Recommends a number of services to which a contact or organisation (who might already be a subscriber or not) can subscribed to. The Web API returns the services as well as their prices for different flows where a contact/organisation is willing to:

Subscribe to their first service or
Subscribe to more services or
Change an existing service (change its price terms or components or change into another service).

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRecommendationSelfServiceResource_getServiceRecommendation" method="get" path="/self-service/v2/services/recommendation" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
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
import {
  recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation,
} from "crm/funcs/recommendations-com-crm-service-recommendation-self-service-resource-get-service-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRecommendationSelfServiceResource_getServiceRecommendation" method="get" path="/self-service/v2/services/recommendation" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
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
import {
  recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation,
} from "crm/funcs/recommendations-com-crm-service-recommendation-self-service-resource-get-service-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRecommendationSelfServiceResource_getServiceRecommendation" method="get" path="/self-service/v2/services/recommendation" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
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
import {
  recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation,
} from "crm/funcs/recommendations-com-crm-service-recommendation-self-service-resource-get-service-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation failed:", res.error);
  }
}

run();
```
### Example Usage: Service Recommendation Response

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRecommendationSelfServiceResource_getServiceRecommendation" method="get" path="/self-service/v2/services/recommendation" example="Service Recommendation Response" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
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
import {
  recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation,
} from "crm/funcs/recommendations-com-crm-service-recommendation-self-service-resource-get-service-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ServiceRecommendationSelfServiceResource_getServiceRecommendation" method="get" path="/self-service/v2/services/recommendation" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.recommendations.comCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
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
import {
  recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation,
} from "crm/funcs/recommendations-com-crm-service-recommendation-self-service-resource-get-service-recommendation.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    includeComponents: true,
    includeCreatives: true,
    searchValue: "coffee",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("recommendationsComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendation failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                        | Type                                                                                                                                                                                                             | Required                                                                                                                                                                                                         | Description                                                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                        | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationRequest](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-request.md)   | :heavy_check_mark:                                                                                                                                                                                               | The request object to use for the request.                                                                                                                                                                       |
| `security`                                                                                                                                                                                                       | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationSecurity](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-security.md) | :heavy_check_mark:                                                                                                                                                                                               | The security requirements to use for the request.                                                                                                                                                                |
| `options`                                                                                                                                                                                                        | RequestOptions                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                               | Used to set various options for making HTTP requests.                                                                                                                                                            |
| `options.fetchOptions`                                                                                                                                                                                           | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                               | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                   |
| `options.retries`                                                                                                                                                                                                | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                               | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                 |

### Response

**Promise\<[operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationResponse](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |