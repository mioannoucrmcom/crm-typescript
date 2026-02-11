# ProductCatalogue

## Overview

Product Catalogue

### Available Operations

* [comCrmProductSelfServiceResourceListProducts](#comcrmproductselfserviceresourcelistproducts) - Search Products
* [comCrmProductSelfServiceResourceGetProduct](#comcrmproductselfserviceresourcegetproduct) - Get Product
* [comCrmProductSelfServiceResourceGetProductComponents](#comcrmproductselfserviceresourcegetproductcomponents) - Get Product Components
* [comCrmProductSelfServiceResourceGetProductVariations](#comcrmproductselfserviceresourcegetproductvariations) - Get Product Variants

## comCrmProductSelfServiceResourceListProducts

Retrieves a list of products that can be purchased by customers through an order, filtered by their category, type etc. Modifier and Variant products are excluded since these product can only be ordered as part of another product and not individually.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: EXPENSE_SERVICE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="EXPENSE_SERVICE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "EXPENSE_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "EXPENSE_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: NON_TRACEABLE_PHYSCAL_GOOD

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="NON_TRACEABLE_PHYSCAL_GOOD" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "NON_TRACEABLE_PHYSCAL_GOOD",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "NON_TRACEABLE_PHYSCAL_GOOD",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: ONE_TME_SERVICE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="ONE_TME_SERVICE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "ONE_TME_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "ONE_TME_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: TERMED_SERVICE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="TERMED_SERVICE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "TERMED_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "TERMED_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: TRACEABLE_PHYSICAL_GOOD

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="TRACEABLE_PHYSICAL_GOOD" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "TRACEABLE_PHYSICAL_GOOD",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "TRACEABLE_PHYSICAL_GOOD",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: USAGE_SERVICE

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="USAGE_SERVICE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "USAGE_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    classification: "USAGE_SERVICE",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: validity_date[gt]

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="validity_date[gt]" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: validity_date[gte]

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="validity_date[gte]" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: false,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: validity_date[lt]

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="validity_date[lt]" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```
### Example Usage: validity_date[lte]

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_listProducts" method="get" path="/self-service/v2/products" example="validity_date[lte]" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceListProducts({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
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
import { productCatalogueComCrmProductSelfServiceResourceListProducts } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-list-products.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceListProducts(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    brandId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryId: "dccb219b-1304-95de-61f8-03b4b824a428",
    categoryIdExact: "dccb219b-1304-95de-61f8-03b4b824a428",
    characteristics: "key;value,key;value",
    composition: "FLAT",
    country: "GBR",
    currency: "EUR",
    customFields: "key;value,key;value",
    familyId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeCharacteristics: true,
    includeCustomFields: true,
    includesOneTimeServices: true,
    instanceModel: "QUANTITY_BASED",
    isModifier: true,
    orderCatalogId: "dccb219b-1304-95de-61f8-03b4b824a428",
    orderCategoryId: "43ft5fb-1304-95de-61f8-03b4b824a428",
    productIds: "dccb219b-1304-95de-61f8-03b4b824a428,8c939607-2262-544d-99ef-4634c6e8836d",
    productSkus: "STB,COF,PIE",
    typeId: "dccb219b-1304-95de-61f8-03b4b824a428",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceListProducts failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceListProductsRequest](../../models/operations/com-crm-product-self-service-resource-list-products-request.md)                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmProductSelfServiceResourceListProductsSecurity](../../models/operations/com-crm-product-self-service-resource-list-products-security.md)                     | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmProductSelfServiceResourceListProductsResponse](../../models/operations/com-crm-product-self-service-resource-list-products-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductSelfServiceResourceGetProduct

Get detailed information of the product, its prices and taxes

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_getProduct" method="get" path="/self-service/v2/products/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceGetProduct({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "8c939607-2262-544d-99ef-4634c6e8836d",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { productCatalogueComCrmProductSelfServiceResourceGetProduct } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-get-product.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceGetProduct(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "8c939607-2262-544d-99ef-4634c6e8836d",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceGetProduct failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceGetProductRequest](../../models/operations/com-crm-product-self-service-resource-get-product-request.md)                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmProductSelfServiceResourceGetProductSecurity](../../models/operations/com-crm-product-self-service-resource-get-product-security.md)                         | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmProductSelfServiceResourceGetProductResponse](../../models/operations/com-crm-product-self-service-resource-get-product-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductSelfServiceResourceGetProductComponents

Returns a list of products that could be added as components of a flexible bundle

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_getProductComponents" method="get" path="/self-service/v2/products/{id}/components" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceGetProductComponents({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "2f6a70b6-84d4-2859-d230-093cb7e95c62",
    characteristics: "key;value,key;value",
    countryCode: "CYP",
    currencyCode: "EUR",
    includeCharacteristics: true,
    includeCustomFields: true,
    includeStock: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { productCatalogueComCrmProductSelfServiceResourceGetProductComponents } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-get-product-components.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceGetProductComponents(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "2f6a70b6-84d4-2859-d230-093cb7e95c62",
    characteristics: "key;value,key;value",
    countryCode: "CYP",
    currencyCode: "EUR",
    includeCharacteristics: true,
    includeCustomFields: true,
    includeStock: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceGetProductComponents failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceGetProductComponentsRequest](../../models/operations/com-crm-product-self-service-resource-get-product-components-request.md)      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmProductSelfServiceResourceGetProductComponentsSecurity](../../models/operations/com-crm-product-self-service-resource-get-product-components-security.md)    | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmProductSelfServiceResourceGetProductComponentsResponse[]](../../models/.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmProductSelfServiceResourceGetProductVariations

Get the detailed information of a composite product’s characteristics, their prices, composition etc. The method can only be used for products classificied as Composite, i.e. they are sold in various variations.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ProductSelfServiceResource_getProductVariations" method="get" path="/self-service/v2/products/{id}/variants" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.productCatalogue.comCrmProductSelfServiceResourceGetProductVariations({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "2f6a70b6-84d4-2859-d230-093cb7e95c62",
    characteristics: "key;value,key;value",
    countryCode: "CYP",
    currencyCode: "EUR",
    includeCharacteristics: true,
    includeStock: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { productCatalogueComCrmProductSelfServiceResourceGetProductVariations } from "crm/funcs/product-catalogue-com-crm-product-self-service-resource-get-product-variations.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await productCatalogueComCrmProductSelfServiceResourceGetProductVariations(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "2f6a70b6-84d4-2859-d230-093cb7e95c62",
    characteristics: "key;value,key;value",
    countryCode: "CYP",
    currencyCode: "EUR",
    includeCharacteristics: true,
    includeStock: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("productCatalogueComCrmProductSelfServiceResourceGetProductVariations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceGetProductVariationsRequest](../../models/operations/com-crm-product-self-service-resource-get-product-variations-request.md)      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmProductSelfServiceResourceGetProductVariationsSecurity](../../models/operations/com-crm-product-self-service-resource-get-product-variations-security.md)    | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmProductSelfServiceResourceGetProductVariationsResponse[]](../../models/.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |