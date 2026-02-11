# ReferralCustomerEvents

## Overview

Referral Customer Events

### Available Operations

* [comCrmReferralCustomerEventSelfServiceResourceCreateReferral](#comcrmreferralcustomereventselfserviceresourcecreatereferral) - Create Referral
* [comCrmReferralCustomerEventSelfServiceResourceReferralActions](#comcrmreferralcustomereventselfserviceresourcereferralactions) - Referral Actions

## comCrmReferralCustomerEventSelfServiceResourceCreateReferral

Create a referral customer event. Such event is created by the front-end application, when a new contact registers and provides the referral code as received by an existing contact's referral

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ReferralCustomerEventSelfServiceResource_createReferral" method="post" path="/self-service/v2/referrals" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.referralCustomerEvents.comCrmReferralCustomerEventSelfServiceResourceCreateReferral({
    code: "REF123",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceCreateReferral,
} from "crmcom/funcs/referral-customer-events-com-crm-referral-customer-event-self-service-resource-create-referral.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceCreateReferral(crmcom, {
    code: "REF123",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceCreateReferral failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                  | Type                                                                                                                                                                                       | Required                                                                                                                                                                                   | Description                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                                  | [operations.ComCrmReferralCustomerEventSelfServiceResourceCreateReferralRequest](../../models/operations/com-crm-referral-customer-event-self-service-resource-create-referral-request.md) | :heavy_check_mark:                                                                                                                                                                         | The request object to use for the request.                                                                                                                                                 |
| `options`                                                                                                                                                                                  | RequestOptions                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                         | Used to set various options for making HTTP requests.                                                                                                                                      |
| `options.fetchOptions`                                                                                                                                                                     | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                    | :heavy_minus_sign:                                                                                                                                                                         | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.             |
| `options.retries`                                                                                                                                                                          | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                         | Enables retrying HTTP requests under certain failure conditions.                                                                                                                           |

### Response

**Promise\<[operations.ComCrmReferralCustomerEventSelfServiceResourceCreateReferralResponse](../../models/operations/com-crm-referral-customer-event-self-service-resource-create-referral-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmReferralCustomerEventSelfServiceResourceReferralActions

Perform referral actions, such as send referrals to contacts inviting them to sign up to a business and in return to award their referred by contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ReferralCustomerEventSelfServiceResource_referralActions" method="post" path="/self-service/v2/referrals/actions" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  await crmcom.referralCustomerEvents.comCrmReferralCustomerEventSelfServiceResourceReferralActions({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    action: "SEND",
    recipients: [
      "0035722265566",
    ],
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceReferralActions,
} from "crmcom/funcs/referral-customer-events-com-crm-referral-customer-event-self-service-resource-referral-actions.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceReferralActions(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    action: "SEND",
    recipients: [
      "0035722265566",
    ],
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("referralCustomerEventsComCrmReferralCustomerEventSelfServiceResourceReferralActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                      | Type                                                                                                                                                                                           | Required                                                                                                                                                                                       | Description                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                      | [operations.ComCrmReferralCustomerEventSelfServiceResourceReferralActionsRequest](../../models/operations/com-crm-referral-customer-event-self-service-resource-referral-actions-request.md)   | :heavy_check_mark:                                                                                                                                                                             | The request object to use for the request.                                                                                                                                                     |
| `security`                                                                                                                                                                                     | [operations.ComCrmReferralCustomerEventSelfServiceResourceReferralActionsSecurity](../../models/operations/com-crm-referral-customer-event-self-service-resource-referral-actions-security.md) | :heavy_check_mark:                                                                                                                                                                             | The security requirements to use for the request.                                                                                                                                              |
| `options`                                                                                                                                                                                      | RequestOptions                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                        | :heavy_minus_sign:                                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                 |
| `options.retries`                                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |