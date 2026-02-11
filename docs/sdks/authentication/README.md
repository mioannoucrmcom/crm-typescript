# Authentication

## Overview

Ability to authenticate customers via a Mobile App or a Portal

### Available Operations

* [comCrmContactSelfServiceResourceAuthenticate](#comcrmcontactselfserviceresourceauthenticate) - Contact Authentication
* [comCrmContactSelfServiceResourceChangeForgottenPassword](#comcrmcontactselfserviceresourcechangeforgottenpassword) - Change Forgotten Password
* [comCrmContactSelfServiceResourceForgotPassword](#comcrmcontactselfserviceresourceforgotpassword) - Forgot Password
* [comCrmContactSelfServiceResourceRequestOTP](#comcrmcontactselfserviceresourcerequestotp) - Request One Time Password
* [comCrmContactSelfServiceResourceRefresh](#comcrmcontactselfserviceresourcerefresh) - Refresh Contact Token
* [comCrmContactSelfServiceResourceEmailVerification](#comcrmcontactselfserviceresourceemailverification) - Request Email Verification
* [comCrmContactSelfServiceResourceValidateOTP](#comcrmcontactselfserviceresourcevalidateotp) - Validate One Time Password
* [comCrmContactSelfServiceResourceVerifyContactEmail](#comcrmcontactselfserviceresourceverifycontactemail) - Verify Contact Email
* [comCrmContactSelfServiceResourceChangePassword](#comcrmcontactselfserviceresourcechangepassword) - Change Password
* [addContactIdentitySS](#addcontactidentityss) - Add Contact Identity
* [comCrmContactSelfServiceResourceSignOut](#comcrmcontactselfserviceresourcesignout) - Sign Out Contact
* [comCrmContactSelfServiceResourceSwitchContact](#comcrmcontactselfserviceresourceswitchcontact) - Contact Switch

## comCrmContactSelfServiceResourceAuthenticate

Authenticate a contact and provide a token for subsequent API access

### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_authenticate" method="post" path="/self-service/v2/contacts/authenticate" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceAuthenticate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "EMAIL",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
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
import { authenticationComCrmContactSelfServiceResourceAuthenticate } from "crm/funcs/authentication-com-crm-contact-self-service-resource-authenticate.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceAuthenticate(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "EMAIL",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceAuthenticate failed:", res.error);
  }
}

run();
```
### Example Usage: Example 2

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_authenticate" method="post" path="/self-service/v2/contacts/authenticate" example="Example 2" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceAuthenticate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "MAC_ADDRESS",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
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
import { authenticationComCrmContactSelfServiceResourceAuthenticate } from "crm/funcs/authentication-com-crm-contact-self-service-resource-authenticate.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceAuthenticate(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "MAC_ADDRESS",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceAuthenticate failed:", res.error);
  }
}

run();
```
### Example Usage: Example 3

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_authenticate" method="post" path="/self-service/v2/contacts/authenticate" example="Example 3" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceAuthenticate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "FACEBOOK",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
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
import { authenticationComCrmContactSelfServiceResourceAuthenticate } from "crm/funcs/authentication-com-crm-contact-self-service-resource-authenticate.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceAuthenticate(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "FACEBOOK",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceAuthenticate failed:", res.error);
  }
}

run();
```
### Example Usage: Example 4

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_authenticate" method="post" path="/self-service/v2/contacts/authenticate" example="Example 4" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceAuthenticate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "PHONE",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
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
import { authenticationComCrmContactSelfServiceResourceAuthenticate } from "crm/funcs/authentication-com-crm-contact-self-service-resource-authenticate.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceAuthenticate(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "PHONE",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceAuthenticate failed:", res.error);
  }
}

run();
```
### Example Usage: Example 5

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_authenticate" method="post" path="/self-service/v2/contacts/authenticate" example="Example 5" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceAuthenticate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "OIDC_OAUTH",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
      code: "c5380ec8-2f3b-43b3-a6c0-fd7245ad68c4.865ef234-417a-47c9-aa25-387fae5af63a.23ab2c39-baad-466c-a514-09cccc012e8f",
      state: "73fdbc26-ed40-43c0-8321-06b42a017385",
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
import { authenticationComCrmContactSelfServiceResourceAuthenticate } from "crm/funcs/authentication-com-crm-contact-self-service-resource-authenticate.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceAuthenticate(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "OIDC_OAUTH",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
      code: "c5380ec8-2f3b-43b3-a6c0-fd7245ad68c4.865ef234-417a-47c9-aa25-387fae5af63a.23ab2c39-baad-466c-a514-09cccc012e8f",
      state: "73fdbc26-ed40-43c0-8321-06b42a017385",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceAuthenticate failed:", res.error);
  }
}

run();
```
### Example Usage: Example 6

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_authenticate" method="post" path="/self-service/v2/contacts/authenticate" example="Example 6" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceAuthenticate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "GOOGLE",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
      code: "4%2F0AeaYSHCFW5hOh7sz-Crq6BuxLalPoja9z9HDkB9KigB7uLyGqVGKpibruxad9J9anRglpw",
      state: "5369d602-1774-45dc-912b-41e299e54a9d",
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
import { authenticationComCrmContactSelfServiceResourceAuthenticate } from "crm/funcs/authentication-com-crm-contact-self-service-resource-authenticate.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceAuthenticate(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    body: {
      provider: "GOOGLE",
      username: "johndoe@crm.com",
      password: "password1234",
      token: "234er43ergt34eett34",
      phone: {
        number: "99000000",
        countryCode: "CYP",
      },
      macAddress: "01-23-45-67-89-AB",
      code: "4%2F0AeaYSHCFW5hOh7sz-Crq6BuxLalPoja9z9HDkB9KigB7uLyGqVGKpibruxad9J9anRglpw",
      state: "5369d602-1774-45dc-912b-41e299e54a9d",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceAuthenticate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceAuthenticateRequest](../../models/operations/com-crm-contact-self-service-resource-authenticate-request.md)                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceAuthenticateSecurity](../../models/operations/com-crm-contact-self-service-resource-authenticate-security.md)                      | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceAuthenticateResponse](../../models/operations/com-crm-contact-self-service-resource-authenticate-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceChangeForgottenPassword

Changes a contact’s password after a password reset request (contact should perform a password reset, where a communication will be sent with a password reset link, and when opening such link and providing new password then this action should be performed)

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_changeForgottenPassword" method="post" path="/self-service/v2/contacts/change_password" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.authentication.comCrmContactSelfServiceResourceChangeForgottenPassword({
    token: "j677enty-23sfsfsf23456798vgp",
    password: "wsxcde421qadfg",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceChangeForgottenPassword } from "crm/funcs/authentication-com-crm-contact-self-service-resource-change-forgotten-password.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceChangeForgottenPassword(crm, {
    token: "j677enty-23sfsfsf23456798vgp",
    password: "wsxcde421qadfg",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceChangeForgottenPassword failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                       | Type                                                                                                                                                                            | Required                                                                                                                                                                        | Description                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceChangeForgottenPasswordRequest](../../models/operations/com-crm-contact-self-service-resource-change-forgotten-password-request.md) | :heavy_check_mark:                                                                                                                                                              | The request object to use for the request.                                                                                                                                      |
| `options`                                                                                                                                                                       | RequestOptions                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                              | Used to set various options for making HTTP requests.                                                                                                                           |
| `options.fetchOptions`                                                                                                                                                          | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                         | :heavy_minus_sign:                                                                                                                                                              | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.  |
| `options.retries`                                                                                                                                                               | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                              | Enables retrying HTTP requests under certain failure conditions.                                                                                                                |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceForgotPassword

Requests a password reset for an existing contact, who forgot his/her password and cannot sign in

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_forgotPassword" method="post" path="/self-service/v2/contacts/forgot_password" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.authentication.comCrmContactSelfServiceResourceForgotPassword({
    body: {
      username: "johndoe@crm.com",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceForgotPassword } from "crm/funcs/authentication-com-crm-contact-self-service-resource-forgot-password.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceForgotPassword(crm, {
    body: {
      username: "johndoe@crm.com",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceForgotPassword failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceForgotPasswordRequest](../../models/operations/com-crm-contact-self-service-resource-forgot-password-request.md)                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceRequestOTP

Request an one time password based on a contact's details

Requesting an one time password will identify a contact based on the provided details (credentials) and once a single contact is found, an outbound communication (SMS or Email) will be send with a 6-digit number that can be used for verifying a contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_requestOTP" method="post" path="/self-service/v2/contacts/otp" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceRequestOTP({
    body: {
      method: "EMAIL",
      credentials: [
        {
          name: "LOYALTY_IDENTIFIER",
          value: "1234567",
        },
        {
          name: "ID_NUMBER",
          value: "100995471",
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
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceRequestOTP } from "crm/funcs/authentication-com-crm-contact-self-service-resource-request-otp.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceRequestOTP(crm, {
    body: {
      method: "EMAIL",
      credentials: [
        {
          name: "LOYALTY_IDENTIFIER",
          value: "1234567",
        },
        {
          name: "ID_NUMBER",
          value: "100995471",
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceRequestOTP failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceRequestOTPRequest](../../models/operations/com-crm-contact-self-service-resource-request-otp-request.md)                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceRequestOTPResponse](../../models/operations/com-crm-contact-self-service-resource-request-otp-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceRefresh

Refresh the contact session based on a “refresh” token and provide an access token that will be used for subsequent API requests

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_refresh" method="post" path="/self-service/v2/contacts/refresh" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceRefresh();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceRefresh } from "crm/funcs/authentication-com-crm-contact-self-service-resource-refresh.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceRefresh(crm);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceRefresh failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceRefreshResponse](../../models/operations/com-crm-contact-self-service-resource-refresh-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceEmailVerification

Request another email verification for a contact after an email verification has been sent, but not verified

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_emailVerification" method="post" path="/self-service/v2/contacts/request_email_verification" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.authentication.comCrmContactSelfServiceResourceEmailVerification({
    body: {
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
import { authenticationComCrmContactSelfServiceResourceEmailVerification } from "crm/funcs/authentication-com-crm-contact-self-service-resource-email-verification.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceEmailVerification(crm, {
    body: {
      emailAddress: "johndoe@crm.com",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceEmailVerification failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceEmailVerificationRequest](../../models/operations/com-crm-contact-self-service-resource-email-verification-request.md)             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceValidateOTP

Verifies that the one time password that was requested is valid

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_validateOTP" method="post" path="/self-service/v2/contacts/validate_otp" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceValidateOTP({
    body: {
      code: "123456",
      authOtp: "47c7-318202dbe45d",
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
import { authenticationComCrmContactSelfServiceResourceValidateOTP } from "crm/funcs/authentication-com-crm-contact-self-service-resource-validate-otp.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceValidateOTP(crm, {
    body: {
      code: "123456",
      authOtp: "47c7-318202dbe45d",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceValidateOTP failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceValidateOTPRequest](../../models/operations/com-crm-contact-self-service-resource-validate-otp-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceValidateOTPResponse](../../models/operations/com-crm-contact-self-service-resource-validate-otp-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceVerifyContactEmail

Verify a contact's email address after an email verification request has been sent to the contact (contact should perform an email verification request, where a communication will be sent to the contact with the email verification link, and upon opening such link then this action should be performed)

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_verifyContactEmail" method="get" path="/self-service/v2/contacts/verify_email" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.authentication.comCrmContactSelfServiceResourceVerifyContactEmail({
    token: "ABCTKN123456798VGP2020",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceVerifyContactEmail } from "crm/funcs/authentication-com-crm-contact-self-service-resource-verify-contact-email.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceVerifyContactEmail(crm, {
    token: "ABCTKN123456798VGP2020",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceVerifyContactEmail failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceVerifyContactEmailRequest](../../models/operations/com-crm-contact-self-service-resource-verify-contact-email-request.md)          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceChangePassword

Changes the password for a contact’s identity (given that contact has already signed-in)

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_changePassword" method="post" path="/self-service/v2/contacts/{id}/change_password" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.authentication.comCrmContactSelfServiceResourceChangePassword({
    id: "a417df7f-d957-c365-fdf9-6093b3eb116c",
    body: {
      password: "wsxcde421qadfg",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceChangePassword } from "crm/funcs/authentication-com-crm-contact-self-service-resource-change-password.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceChangePassword(crm, {
    id: "a417df7f-d957-c365-fdf9-6093b3eb116c",
    body: {
      password: "wsxcde421qadfg",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceChangePassword failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceChangePasswordRequest](../../models/operations/com-crm-contact-self-service-resource-change-password-request.md)                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## addContactIdentitySS

Create a new contact identity that will be used when authenticating contacts during sign-ins. Use this Web API when contacts, already registered in CRM.COM, access the self-service for the first time in order to create their authentication information.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="addContactIdentitySS" method="post" path="/self-service/v2/contacts/{id}/identities" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.authentication.addContactIdentitySS({
    id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
    body: {
      provider: "EMAIL",
      email: "johndoe@crm.com",
      password: "1123123rerwr",
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
import { authenticationAddContactIdentitySS } from "crm/funcs/authentication-add-contact-identity-ss.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationAddContactIdentitySS(crm, {
    id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
    body: {
      provider: "EMAIL",
      email: "johndoe@crm.com",
      password: "1123123rerwr",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationAddContactIdentitySS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AddContactIdentitySSRequest](../../models/operations/add-contact-identity-ss-request.md)                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AddContactIdentitySSResponse](../../models/operations/add-contact-identity-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceSignOut

Signs out a contact by terminating his/her session, such contact will not be able to access the client (application) and should sign in again in order to do so

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_signOut" method="post" path="/self-service/v2/contacts/{id}/sign_out" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.authentication.comCrmContactSelfServiceResourceSignOut({
    id: "9781d1db-38db-598f-2bb5-a3de3fbc2730",
    body: {},
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceSignOut } from "crm/funcs/authentication-com-crm-contact-self-service-resource-sign-out.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceSignOut(crm, {
    id: "9781d1db-38db-598f-2bb5-a3de3fbc2730",
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceSignOut failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceSignOutRequest](../../models/operations/com-crm-contact-self-service-resource-sign-out-request.md)                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceSwitchContact

Switch a contact to another contact that is related to, being part of such contact's community

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_switchContact" method="post" path="/self-service/v2/contacts/{id}/switch" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.authentication.comCrmContactSelfServiceResourceSwitchContact({
    id: "0362aa5b-4438-deb0-b56b-1974f6a27c7f",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { authenticationComCrmContactSelfServiceResourceSwitchContact } from "crm/funcs/authentication-com-crm-contact-self-service-resource-switch-contact.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await authenticationComCrmContactSelfServiceResourceSwitchContact(crm, {
    id: "0362aa5b-4438-deb0-b56b-1974f6a27c7f",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("authenticationComCrmContactSelfServiceResourceSwitchContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceSwitchContactRequest](../../models/operations/com-crm-contact-self-service-resource-switch-contact-request.md)                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceSwitchContactResponse](../../models/operations/com-crm-contact-self-service-resource-switch-contact-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |