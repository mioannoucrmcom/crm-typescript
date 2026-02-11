# OrderCatalogues

## Overview

Order Catalogues

### Available Operations

* [comCrmOrderCatalogSelfServiceResourceList](#comcrmordercatalogselfserviceresourcelist) - List Order Catalogues
* [comCrmOrderCatalogSelfServiceResourceListCategories](#comcrmordercatalogselfserviceresourcelistcategories) - List Order Catalogue Categories

## comCrmOrderCatalogSelfServiceResourceList

Returns a list of active order catalogues. By default all Order Catalogues are included in the list, but this list can be shorten using the filters such as the time of ordering or the organisation that fulfills the order to be placed. In addition, order catalogues owned by specified organisations are available only when that organisation fulfills an order and this cannot be restricted/overridden by the API's filters.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_list" method="get" path="/self-service/v2/order_catalogues" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceList({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
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
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceList } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceList(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_list" method="get" path="/self-service/v2/order_catalogues" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceList({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
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
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceList } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceList(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_list" method="get" path="/self-service/v2/order_catalogues" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceList({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
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
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceList } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceList(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_list" method="get" path="/self-service/v2/order_catalogues" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceList({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
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
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceList } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceList(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_list" method="get" path="/self-service/v2/order_catalogues" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceList({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
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
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceList } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceList(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    fulfilledBy: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    orderCatalogIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    orderingTime: 1644574218,
    searchValue: "Food",
    supplyMethod: "DELIVERY",
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrderCatalogSelfServiceResourceListRequest](../../models/operations/com-crm-order-catalog-self-service-resource-list-request.md)                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmOrderCatalogSelfServiceResourceListSecurity](../../models/operations/com-crm-order-catalog-self-service-resource-list-security.md)                           | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrderCatalogSelfServiceResourceListResponse](../../models/operations/com-crm-order-catalog-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrderCatalogSelfServiceResourceListCategories

Returns a list of order catalogue categories and the products under each one of these categories. By default, the Web API returns the root catagories within the categories structure. Use sub-sequent calls to the same Web API to get each category's child nodes

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_listCategories" method="get" path="/self-service/v2/order_catalogues/{id}/categories" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceListCategories({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { CrmcomCore } from "crmcom/core.js";
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list-categories.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_listCategories" method="get" path="/self-service/v2/order_catalogues/{id}/categories" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceListCategories({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { CrmcomCore } from "crmcom/core.js";
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list-categories.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
    parentId: "9365d945-2c62-be0e-a8dc-45736fdfa5b5",
    returnAll: true,
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_listCategories" method="get" path="/self-service/v2/order_catalogues/{id}/categories" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceListCategories({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { CrmcomCore } from "crmcom/core.js";
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list-categories.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_listCategories" method="get" path="/self-service/v2/order_catalogues/{id}/categories" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceListCategories({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { CrmcomCore } from "crmcom/core.js";
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list-categories.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderCatalogSelfServiceResource_listCategories" method="get" path="/self-service/v2/order_catalogues/{id}/categories" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.orderCatalogues.comCrmOrderCatalogSelfServiceResourceListCategories({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
import { CrmcomCore } from "crmcom/core.js";
import { orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories } from "crmcom/funcs/order-catalogues-com-crm-order-catalog-self-service-resource-list-categories.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
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
    console.log("orderCataloguesComCrmOrderCatalogSelfServiceResourceListCategories failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrderCatalogSelfServiceResourceListCategoriesRequest](../../models/operations/com-crm-order-catalog-self-service-resource-list-categories-request.md)        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmOrderCatalogSelfServiceResourceListCategoriesSecurity](../../models/operations/com-crm-order-catalog-self-service-resource-list-categories-security.md)      | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrderCatalogSelfServiceResourceListCategoriesResponse](../../models/operations/com-crm-order-catalog-self-service-resource-list-categories-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |