# Contact

## Overview

Contact

### Available Operations

* [comCrmContactSelfServiceResourceVerifyContactExists](#comcrmcontactselfserviceresourceverifycontactexists) - Verify Contact Existence
* [comCrmContactSelfServiceResourceGetOIDCConfiguration](#comcrmcontactselfserviceresourcegetoidcconfiguration) - OIDC Contact Authentication
* [registerContactSS](#registercontactss) - Register Contact
* [getSingleContactSS](#getsinglecontactss) - Get Contact
* [updateContactSS](#updatecontactss) - Update Contact
* [comCrmContactSelfServiceResourceUnregisterContact](#comcrmcontactselfserviceresourceunregistercontact) - Unregister Contact
* [comCrmAccountSelfServiceResourceExportStatement](#comcrmaccountselfserviceresourceexportstatement) - Export Statement
* [comCrmContactSelfServiceResourceAction](#comcrmcontactselfserviceresourceaction) - Perform Community Invitation Actions

## comCrmContactSelfServiceResourceVerifyContactExists

Verify the existence of a contact using either their email or phone. The result is a boolean value.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_verifyContactExists" method="get" path="/self-service/v2/contacts" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contact.comCrmContactSelfServiceResourceVerifyContactExists({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    emailAddress: "john@gmail.com",
    phone: "99123456",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactComCrmContactSelfServiceResourceVerifyContactExists } from "crmcom/funcs/contact-com-crm-contact-self-service-resource-verify-contact-exists.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactComCrmContactSelfServiceResourceVerifyContactExists(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    emailAddress: "john@gmail.com",
    phone: "99123456",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactComCrmContactSelfServiceResourceVerifyContactExists failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceVerifyContactExistsRequest](../../models/operations/com-crm-contact-self-service-resource-verify-contact-exists-request.md)        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceVerifyContactExistsSecurity](../../models/operations/com-crm-contact-self-service-resource-verify-contact-exists-security.md)      | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceVerifyContactExistsResponse](../../models/operations/com-crm-contact-self-service-resource-verify-contact-exists-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetOIDCConfiguration

Authenticate a contact via on OpenID Connect provider. Web API can be used considering that the contact's credentials are already created on the provider's side.

### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getOIDCConfiguration" method="get" path="/self-service/v2/contacts/oidc/{type}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contact.comCrmContactSelfServiceResourceGetOIDCConfiguration({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    type: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactComCrmContactSelfServiceResourceGetOIDCConfiguration } from "crmcom/funcs/contact-com-crm-contact-self-service-resource-get-oidc-configuration.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactComCrmContactSelfServiceResourceGetOIDCConfiguration(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    type: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactComCrmContactSelfServiceResourceGetOIDCConfiguration failed:", res.error);
  }
}

run();
```
### Example Usage: Example 2

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getOIDCConfiguration" method="get" path="/self-service/v2/contacts/oidc/{type}" example="Example 2" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contact.comCrmContactSelfServiceResourceGetOIDCConfiguration({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    type: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactComCrmContactSelfServiceResourceGetOIDCConfiguration } from "crmcom/funcs/contact-com-crm-contact-self-service-resource-get-oidc-configuration.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactComCrmContactSelfServiceResourceGetOIDCConfiguration(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    type: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactComCrmContactSelfServiceResourceGetOIDCConfiguration failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetOIDCConfigurationRequest](../../models/operations/com-crm-contact-self-service-resource-get-oidc-configuration-request.md)      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceGetOIDCConfigurationSecurity](../../models/operations/com-crm-contact-self-service-resource-get-oidc-configuration-security.md)    | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetOIDCConfigurationResponse](../../models/operations/com-crm-contact-self-service-resource-get-oidc-configuration-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## registerContactSS

<div class="description spec-item__description"><p>Create a new contact of type ‘person’. A contact is created as part of the contact registration process via an app or portal. Contacts can register and authenticate their registration using one of the following methods subject to configuration:</p>
<ul>
<li>email &amp; password</li>
<li>email &amp; OTP</li>
<li>phone &amp; OTP</li>
<li>Facebook</li>
<li>Google</li>
</ul>
</div>

### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="registerContactSS" method="post" path="/self-service/v2/contacts/register" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contact.registerContactSS({
    apiKey: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    body: {
      firstName: "John",
      lastName: "Doe",
      identification: {
        provider: "FACEBOOK",
        email: "johndoe@crm.com",
        password: "123456",
        phone: {
          number: "99123456",
          countryCode: "CYP",
        },
        applicationId: "3c33dcc6-3958-4e7d-ae0e-592948627711",
        token: "YOJDAKEb9l1U0sUzrskM6X4emzrSeXqb",
      },
      emailOptOut: true,
      smsOptOut: true,
      referralCode: "3M5Y1P",
      customFields: [
        {
          key: "custom_key",
          value: "0001-345",
        },
      ],
      languageCode: "IT",
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
import { contactRegisterContactSS } from "crmcom/funcs/contact-register-contact-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRegisterContactSS(crmcom, {
    apiKey: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    body: {
      firstName: "John",
      lastName: "Doe",
      identification: {
        provider: "FACEBOOK",
        email: "johndoe@crm.com",
        password: "123456",
        phone: {
          number: "99123456",
          countryCode: "CYP",
        },
        applicationId: "3c33dcc6-3958-4e7d-ae0e-592948627711",
        token: "YOJDAKEb9l1U0sUzrskM6X4emzrSeXqb",
      },
      emailOptOut: true,
      smsOptOut: true,
      referralCode: "3M5Y1P",
      customFields: [
        {
          key: "custom_key",
          value: "0001-345",
        },
      ],
      languageCode: "IT",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactRegisterContactSS failed:", res.error);
  }
}

run();
```
### Example Usage: Example 2

<!-- UsageSnippet language="typescript" operationID="registerContactSS" method="post" path="/self-service/v2/contacts/register" example="Example 2" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contact.registerContactSS({
    apiKey: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    body: {
      firstName: "John",
      lastName: "Doe",
      identification: {
        provider: "PHONE",
        email: "johndoe@crm.com",
      },
      emailOptOut: true,
      smsOptOut: true,
      languageCode: "IT",
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
import { contactRegisterContactSS } from "crmcom/funcs/contact-register-contact-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactRegisterContactSS(crmcom, {
    apiKey: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    body: {
      firstName: "John",
      lastName: "Doe",
      identification: {
        provider: "PHONE",
        email: "johndoe@crm.com",
      },
      emailOptOut: true,
      smsOptOut: true,
      languageCode: "IT",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactRegisterContactSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.RegisterContactSSRequest](../../models/operations/register-contact-ss-request.md)                                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.RegisterContactSSResponse](../../models/operations/register-contact-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## getSingleContactSS

Retrieve basic information for a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSingleContactSS" method="get" path="/self-service/v2/contacts/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contact.getSingleContactSS({
    id: "6e2f83ca-69e9-4ea4-96c5-73a4c641979d",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactGetSingleContactSS } from "crmcom/funcs/contact-get-single-contact-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactGetSingleContactSS(crmcom, {
    id: "6e2f83ca-69e9-4ea4-96c5-73a4c641979d",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactGetSingleContactSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSingleContactSSRequest](../../models/operations/get-single-contact-ss-request.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSingleContactSSResponse](../../models/operations/get-single-contact-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## updateContactSS

Update information for an existing contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateContactSS" method="put" path="/self-service/v2/contacts/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contact.updateContactSS({
    id: "e2ade504-9b90-92be-0adb-3258475ff695",
    body: {
      firstName: "John",
      middleName: "Patrick",
      lastName: "Smith",
      languageCode: "ENG",
      email: "john.smith@gmail.com",
      demographics: {
        gender: "MALE",
        dateOfBirth: {
          year: 1948,
          month: 3,
          day: 1,
        },
        nameDay: {
          month: 8,
          day: 6,
        },
      },
      smsOptOut: false,
      emailOptOut: false,
      customFields: [
        {
          key: "custom_key",
          value: "0001-345",
        },
      ],
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
import { contactUpdateContactSS } from "crmcom/funcs/contact-update-contact-ss.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactUpdateContactSS(crmcom, {
    id: "e2ade504-9b90-92be-0adb-3258475ff695",
    body: {
      firstName: "John",
      middleName: "Patrick",
      lastName: "Smith",
      languageCode: "ENG",
      email: "john.smith@gmail.com",
      demographics: {
        gender: "MALE",
        dateOfBirth: {
          year: 1948,
          month: 3,
          day: 1,
        },
        nameDay: {
          month: 8,
          day: 6,
        },
      },
      smsOptOut: false,
      emailOptOut: false,
      customFields: [
        {
          key: "custom_key",
          value: "0001-345",
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactUpdateContactSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateContactSSRequest](../../models/operations/update-contact-ss-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateContactSSResponse](../../models/operations/update-contact-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceUnregisterContact

Unregisters a contact from a business

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_unregisterContact" method="delete" path="/self-service/v2/contacts/{id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  await crmcom.contact.comCrmContactSelfServiceResourceUnregisterContact({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "e18ee2bc-c6f3-49e1-8e05-763386378017",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactComCrmContactSelfServiceResourceUnregisterContact } from "crmcom/funcs/contact-com-crm-contact-self-service-resource-unregister-contact.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactComCrmContactSelfServiceResourceUnregisterContact(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "e18ee2bc-c6f3-49e1-8e05-763386378017",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactComCrmContactSelfServiceResourceUnregisterContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceUnregisterContactRequest](../../models/operations/com-crm-contact-self-service-resource-unregister-contact-request.md)             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceUnregisterContactSecurity](../../models/operations/com-crm-contact-self-service-resource-unregister-contact-security.md)           | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAccountSelfServiceResourceExportStatement

Request (and retrieve) a contact statement

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AccountSelfServiceResource_exportStatement" method="post" path="/self-service/v2/contacts/{id}/export_statement" example="Export Statement" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.contact.comCrmAccountSelfServiceResourceExportStatement({
    id: "b2490476-fc6b-604c-e3f9-5ddd0777efbe",
    body: {
      accountId: "4c0ea630-2972-7714-a5d1-7576b8dc9c22",
      format: "PDF",
      fromMonth: 12,
      fromYear: 2021,
      toMonth: 12,
      toYear: 2022,
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactComCrmAccountSelfServiceResourceExportStatement } from "crmcom/funcs/contact-com-crm-account-self-service-resource-export-statement.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactComCrmAccountSelfServiceResourceExportStatement(crmcom, {
    id: "b2490476-fc6b-604c-e3f9-5ddd0777efbe",
    body: {
      accountId: "4c0ea630-2972-7714-a5d1-7576b8dc9c22",
      format: "PDF",
      fromMonth: 12,
      fromYear: 2021,
      toMonth: 12,
      toYear: 2022,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactComCrmAccountSelfServiceResourceExportStatement failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAccountSelfServiceResourceExportStatementRequest](../../models/operations/com-crm-account-self-service-resource-export-statement-request.md)                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceAction

This API allows a contact to respond to an invitation to join another contact’s community. 

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_action" method="post" path="/self-service/v2/contacts/{id}/people/{relationship_id}/actions" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contact.comCrmContactSelfServiceResourceAction({
    id: "d24a32fd-fac8-3bc0-66a1-533ae7c4707f",
    relationshipId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    body: {
      action: "ACCEPT",
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
import { contactComCrmContactSelfServiceResourceAction } from "crmcom/funcs/contact-com-crm-contact-self-service-resource-action.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactComCrmContactSelfServiceResourceAction(crmcom, {
    id: "d24a32fd-fac8-3bc0-66a1-533ae7c4707f",
    relationshipId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    body: {
      action: "ACCEPT",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactComCrmContactSelfServiceResourceAction failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceActionRequest](../../models/operations/com-crm-contact-self-service-resource-action-request.md)                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceActionResponse](../../models/operations/com-crm-contact-self-service-resource-action-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |