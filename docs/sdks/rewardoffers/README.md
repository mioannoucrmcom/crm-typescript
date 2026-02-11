# RewardOffers

## Overview

Reward Offers

### Available Operations

* [comCrmRewardOfferSelfServiceResourceList](#comcrmrewardofferselfserviceresourcelist) - Search Reward Offers
* [comCrmRewardOfferSelfServiceResourceGetSingle](#comcrmrewardofferselfserviceresourcegetsingle) - Get Reward Offer
* [comCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance](#comcrmrewardofferselfserviceresourcegetrewardofferperformance) - Get Reward Offer Performance

## comCrmRewardOfferSelfServiceResourceList

Retrieve all active reward offers that are applicable for a specific contact

### Example Usage: ACHIEVEMENT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="ACHIEVEMENT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    goals: "ACHIEVEMENT",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "ACHIEVEMENT",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    goals: "ACHIEVEMENT",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "ACHIEVEMENT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: BUNDLE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="BUNDLE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "BUNDLE",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "BUNDLE",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DEFAULT_SORTING",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DEFAULT_SORTING",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: DEFAULT_SORTING

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="DEFAULT_SORTING" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DEFAULT_SORTING",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DEFAULT_SORTING",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: DISCOUNT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="DISCOUNT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "DISCOUNT",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "DISCOUNT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: DISTANCE 

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="DISTANCE " -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DISTANCE",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DISTANCE",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: GIFT

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="GIFT" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "GIFT",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "GIFT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: HAPPYHOUR

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="HAPPYHOUR" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "HAPPYHOUR",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "HAPPYHOUR",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: LOTTERY

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="LOTTERY" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "LOTTERY",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "LOTTERY",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: MEMBERSHIP

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="MEMBERSHIP" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    goals: "MEMBERSHIP",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    goals: "MEMBERSHIP",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DISTANCE",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DISTANCE",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: ORGANISATION_NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="ORGANISATION_NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "ORGANISATION_NAME",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "ORGANISATION_NAME",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: POSTED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="POSTED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "ORGANISATION_NAME",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "ORGANISATION_NAME",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: PROFILE

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="PROFILE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "PROFILE",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "PROFILE",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: REACH_TIER

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="REACH_TIER" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "REACH_TIER",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "REACH_TIER",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: REFER

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="REFER" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "REFER",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "REFER",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SIGNUP

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="SIGNUP" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "SIGNUP",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "SIGNUP",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SPEND

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="SPEND" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    goals: "SPEND",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    goals: "SPEND",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SUBSCRIPTION_MATURITY

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="SUBSCRIPTION_MATURITY" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "SUBSCRIPTION_MATURITY",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    types: "SUBSCRIPTION_MATURITY",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE 

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="UPDATED_DATE " -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DEFAULT_SORTING",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    sort: "DEFAULT_SORTING",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: VISITS

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_list" method="get" path="/self-service/v2/reward_offers" example="VISITS" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceList({
    goals: "VISITS",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
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
import { rewardOffersComCrmRewardOfferSelfServiceResourceList } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceList(crmcom, {
    goals: "VISITS",
    isFeatured: true,
    lat: "35.1730837",
    lon: "33.3761312",
    performanceEnabled: true,
    searchValue: "Increase Visits",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmRewardOfferSelfServiceResourceListRequest](../../models/operations/com-crm-reward-offer-self-service-resource-list-request.md)                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmRewardOfferSelfServiceResourceListResponse](../../models/operations/com-crm-reward-offer-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmRewardOfferSelfServiceResourceGetSingle

Retrieve detailed information for a reward offer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_getSingle" method="get" path="/self-service/v2/reward_offers/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceGetSingle({
    id: "6883441e-194a-b92b-c6c0-2f0e869e4c65",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { rewardOffersComCrmRewardOfferSelfServiceResourceGetSingle } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-get-single.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceGetSingle(crmcom, {
    id: "6883441e-194a-b92b-c6c0-2f0e869e4c65",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleRequest](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-request.md)                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmRewardOfferSelfServiceResourceGetSingleResponse](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance

Retrieve the performance for a specific reward offer (e.g. for every 100 euros worth of purchased goods, get 10 euros back)

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardOfferSelfServiceResource_getRewardOfferPerformance" method="get" path="/self-service/v2/reward_offers/{id}/performance" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.rewardOffers.comCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance({
    id: "a690caa5-9c4d-4eb0-b743-88076f1f5711",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { rewardOffersComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance } from "crmcom/funcs/reward-offers-com-crm-reward-offer-self-service-resource-get-reward-offer-performance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardOffersComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance(crmcom, {
    id: "a690caa5-9c4d-4eb0-b743-88076f1f5711",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardOffersComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                     | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                     | [operations.ComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformanceRequest](../../models/operations/com-crm-reward-offer-self-service-resource-get-reward-offer-performance-request.md) | :heavy_check_mark:                                                                                                                                                                            | The request object to use for the request.                                                                                                                                                    |
| `options`                                                                                                                                                                                     | RequestOptions                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                            | Used to set various options for making HTTP requests.                                                                                                                                         |
| `options.fetchOptions`                                                                                                                                                                        | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                       | :heavy_minus_sign:                                                                                                                                                                            | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                |
| `options.retries`                                                                                                                                                                             | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                            | Enables retrying HTTP requests under certain failure conditions.                                                                                                                              |

### Response

**Promise\<[operations.ComCrmRewardOfferSelfServiceResourceGetRewardOfferPerformanceResponse](../../models/operations/com-crm-reward-offer-self-service-resource-get-reward-offer-performance-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |