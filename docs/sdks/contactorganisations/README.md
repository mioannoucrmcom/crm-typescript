# ContactOrganisations

## Overview

Contact Organisations

### Available Operations

* [comCrmContactSelfServiceResourceGetOrganisations](#comcrmcontactselfserviceresourcegetorganisations) - Get Contact Organisations
* [signUpOutOrganisationSS](#signupoutorganisationss) - Sign Up/Out Organisation

## comCrmContactSelfServiceResourceGetOrganisations

Retrieves all organisations that the contact is signed up to

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getOrganisations" method="get" path="/self-service/v2/contacts/{id}/organisations" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactOrganisations.comCrmContactSelfServiceResourceGetOrganisations({
    id: "<id>",
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
import { contactOrganisationsComCrmContactSelfServiceResourceGetOrganisations } from "crm/funcs/contact-organisations-com-crm-contact-self-service-resource-get-organisations.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactOrganisationsComCrmContactSelfServiceResourceGetOrganisations(crm, {
    id: "<id>",
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactOrganisationsComCrmContactSelfServiceResourceGetOrganisations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetOrganisationsRequest](../../models/operations/com-crm-contact-self-service-resource-get-organisations-request.md)               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetOrganisationsResponse](../../models/operations/com-crm-contact-self-service-resource-get-organisations-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## signUpOutOrganisationSS

Sign-up or sign-out a contact from an existing organisation, used in cases where a Service Owner owns a contact registry.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="signUpOutOrganisationSS" method="post" path="/self-service/v2/contacts/{id}/organisations" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactOrganisations.signUpOutOrganisationSS({
    id: "<id>",
    body: {
      action: "SIGNUP",
      organisationId: "9086dd6b-2b9f-4fba-85ff-1b89143a56da",
      emailOptOut: true,
      smsOptOut: true,
      referralCode: "1234",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactOrganisationsSignUpOutOrganisationSS } from "crm/funcs/contact-organisations-sign-up-out-organisation-ss.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactOrganisationsSignUpOutOrganisationSS(crm, {
    id: "<id>",
    body: {
      action: "SIGNUP",
      organisationId: "9086dd6b-2b9f-4fba-85ff-1b89143a56da",
      emailOptOut: true,
      smsOptOut: true,
      referralCode: "1234",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactOrganisationsSignUpOutOrganisationSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.SignUpOutOrganisationSSRequest](../../models/operations/sign-up-out-organisation-ss-request.md)                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.SignUpOutOrganisationSSResponse](../../models/operations/sign-up-out-organisation-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |