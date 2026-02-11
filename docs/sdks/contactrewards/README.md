# ContactRewards

## Overview

Contact Rewards API

### Available Operations

* [comCrmContactSelfServiceResourceVerifySignUp](#comcrmcontactselfserviceresourceverifysignup) - Verify Closed Loop Scheme Request
* [comCrmContactSelfServiceResourceSignUpOutScheme](#comcrmcontactselfserviceresourcesignupoutscheme) - Contact Reward Schemes Actions
* [comCrmContactSelfServiceResourceGetSingleWithRewards](#comcrmcontactselfserviceresourcegetsinglewithrewards) - Get Contact Rewards

## comCrmContactSelfServiceResourceVerifySignUp

Verify a contact's request to sign up to a closed loop reward scheme

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_verifySignUp" method="get" path="/self-service/v2/contacts/reward_schemes/verification/{sign_up_code}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactRewards.comCrmContactSelfServiceResourceVerifySignUp({
    signUpCode: "SUC1234",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactRewardsComCrmContactSelfServiceResourceVerifySignUp } from "crm/funcs/contact-rewards-com-crm-contact-self-service-resource-verify-sign-up.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRewardsComCrmContactSelfServiceResourceVerifySignUp(crm, {
    signUpCode: "SUC1234",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactRewardsComCrmContactSelfServiceResourceVerifySignUp failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceVerifySignUpRequest](../../models/operations/com-crm-contact-self-service-resource-verify-sign-up-request.md)                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceSignUpOutScheme

Sign up/out a contact from/to a reward scheme

### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_signUpOutScheme" method="post" path="/self-service/v2/contacts/{id}/reward_schemes" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactRewards.comCrmContactSelfServiceResourceSignUpOutScheme({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      action: "SIGN_UP",
      rewardSchemeId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme } from "crm/funcs/contact-rewards-com-crm-contact-self-service-resource-sign-up-out-scheme.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme(crm, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      action: "SIGN_UP",
      rewardSchemeId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme failed:", res.error);
  }
}

run();
```
### Example Usage: Example 2

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_signUpOutScheme" method="post" path="/self-service/v2/contacts/{id}/reward_schemes" example="Example 2" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactRewards.comCrmContactSelfServiceResourceSignUpOutScheme({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      action: "SIGN_OUT",
      rewardSchemeId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme } from "crm/funcs/contact-rewards-com-crm-contact-self-service-resource-sign-up-out-scheme.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme(crm, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      action: "SIGN_OUT",
      rewardSchemeId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme failed:", res.error);
  }
}

run();
```
### Example Usage: Example 3

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_signUpOutScheme" method="post" path="/self-service/v2/contacts/{id}/reward_schemes" example="Example 3" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactRewards.comCrmContactSelfServiceResourceSignUpOutScheme({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      action: "SIGN_UP",
      rewardSchemeId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      emailAddress: "johndoe@crm.com",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme } from "crm/funcs/contact-rewards-com-crm-contact-self-service-resource-sign-up-out-scheme.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme(crm, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      action: "SIGN_UP",
      rewardSchemeId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      emailAddress: "johndoe@crm.com",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactRewardsComCrmContactSelfServiceResourceSignUpOutScheme failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceSignUpOutSchemeRequest](../../models/operations/com-crm-contact-self-service-resource-sign-up-out-scheme-request.md)               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetSingleWithRewards

Retrieve a contact's reward details

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getSingleWithRewards" method="get" path="/self-service/v2/contacts/{id}/rewards" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactRewards.comCrmContactSelfServiceResourceGetSingleWithRewards({
    id: "a12b282f-e6ce-e618-0a72-becb3ad78033",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactRewardsComCrmContactSelfServiceResourceGetSingleWithRewards } from "crm/funcs/contact-rewards-com-crm-contact-self-service-resource-get-single-with-rewards.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRewardsComCrmContactSelfServiceResourceGetSingleWithRewards(crm, {
    id: "a12b282f-e6ce-e618-0a72-becb3ad78033",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactRewardsComCrmContactSelfServiceResourceGetSingleWithRewards failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetSingleWithRewardsRequest](../../models/operations/com-crm-contact-self-service-resource-get-single-with-rewards-request.md)     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetSingleWithRewardsResponse](../../models/operations/com-crm-contact-self-service-resource-get-single-with-rewards-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |