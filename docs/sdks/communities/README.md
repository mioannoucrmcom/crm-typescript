# Communities

## Overview

Communities

### Available Operations

* [comCrmContactSettingSelfServiceResourceListCommunityRelations](#comcrmcontactsettingselfserviceresourcelistcommunityrelations) - List Community Relations
* [comCrmContactSelfServiceResourceGetContactCommunitySummaryResults](#comcrmcontactselfserviceresourcegetcontactcommunitysummaryresults) - Get Conmmunity members
* [comCrmContactSelfServiceResourceGetCommunities](#comcrmcontactselfserviceresourcegetcommunities) - List Contact's Communities
* [comCrmContactSelfServiceResourceLeaveCommunity](#comcrmcontactselfserviceresourceleavecommunity) - Leave from Community
* [comCrmContactSelfServiceResourceListContactGroups](#comcrmcontactselfserviceresourcelistcontactgroups) - List Contact's Groups
* [comCrmContactSelfServiceResourceUpdateContactGroupName](#comcrmcontactselfserviceresourceupdatecontactgroupname) - Update Contact Group Name
* [comCrmContactSelfServiceResourceListContactRelationship](#comcrmcontactselfserviceresourcelistcontactrelationship) - List Community People
* [comCrmContactSelfServiceResourceAddContactRelationship](#comcrmcontactselfserviceresourceaddcontactrelationship) - Add Community Person
* [comCrmContactSelfServiceResourceGetContactRelationship](#comcrmcontactselfserviceresourcegetcontactrelationship) - Retrieve Community Person
* [comCrmContactSelfServiceResourceUpdateContactRelationship](#comcrmcontactselfserviceresourceupdatecontactrelationship) - Update Community Person
* [comCrmContactSelfServiceResourceRemoveContactRelationship](#comcrmcontactselfserviceresourceremovecontactrelationship) - Delete Community Person
* [comCrmContactSelfServiceResourceGetContactPersonAllowance](#comcrmcontactselfserviceresourcegetcontactpersonallowance) - Retrieve Community Person product allowance
* [comCrmContactSelfServiceResourceAddContactRelationshipProductAllowance](#comcrmcontactselfserviceresourceaddcontactrelationshipproductallowance) - Add Community Person product allowance
* [comCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance](#comcrmcontactselfserviceresourceupdatecontactrelationshipproductallowance) - Update Community Person product allowance
* [comCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance](#comcrmcontactselfserviceresourceremovecontactrelationshipproductallowance) - Delete Community Person allowance product
* [comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance](#comcrmcontactselfserviceresourcegetcontactpersonremainingallowance) - Retrieve Community Person remaining product allowance

## comCrmContactSettingSelfServiceResourceListCommunityRelations

Retrieve a list of contact community relations based on search criteria (e.g. all contact community relations)


### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSettingSelfServiceResource_listCommunityRelations" method="get" path="/self-service/v2/communities/relations" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSettingSelfServiceResourceListCommunityRelations({
    includeTotal: true,
    name: "Employees",
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSettingSelfServiceResourceListCommunityRelations } from "crmcom/funcs/communities-com-crm-contact-setting-self-service-resource-list-community-relations.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSettingSelfServiceResourceListCommunityRelations(crmcom, {
    includeTotal: true,
    name: "Employees",
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSettingSelfServiceResourceListCommunityRelations failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                    | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                    | [operations.ComCrmContactSettingSelfServiceResourceListCommunityRelationsRequest](../../models/operations/com-crm-contact-setting-self-service-resource-list-community-relations-request.md) | :heavy_check_mark:                                                                                                                                                                           | The request object to use for the request.                                                                                                                                                   |
| `options`                                                                                                                                                                                    | RequestOptions                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                           | Used to set various options for making HTTP requests.                                                                                                                                        |
| `options.fetchOptions`                                                                                                                                                                       | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                      | :heavy_minus_sign:                                                                                                                                                                           | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.               |
| `options.retries`                                                                                                                                                                            | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                           | Enables retrying HTTP requests under certain failure conditions.                                                                                                                             |

### Response

**Promise\<[operations.ComCrmContactSettingSelfServiceResourceListCommunityRelationsResponse](../../models/operations/com-crm-contact-setting-self-service-resource-list-community-relations-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetContactCommunitySummaryResults

Retrieves all the community members (ones who either accepted the invitation or have pending invitation).

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactCommunitySummaryResults" method="get" path="/self-service/v2/contacts/community/members" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactCommunitySummaryResults({
    group: "<value>",
    includeTotal: true,
    ownerId: "<id>",
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceGetContactCommunitySummaryResults } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-community-summary-results.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactCommunitySummaryResults(crmcom, {
    group: "<value>",
    includeTotal: true,
    ownerId: "<id>",
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactCommunitySummaryResults failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                             | Type                                                                                                                                                                                                  | Required                                                                                                                                                                                              | Description                                                                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsRequest](../../models/operations/com-crm-contact-self-service-resource-get-contact-community-summary-results-request.md) | :heavy_check_mark:                                                                                                                                                                                    | The request object to use for the request.                                                                                                                                                            |
| `options`                                                                                                                                                                                             | RequestOptions                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                    | Used to set various options for making HTTP requests.                                                                                                                                                 |
| `options.fetchOptions`                                                                                                                                                                                | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                    | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                        |
| `options.retries`                                                                                                                                                                                     | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                    | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                      |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsResponse](../../models/operations/com-crm-contact-self-service-resource-get-contact-community-summary-results-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetCommunities

Lists all communities that a contact is a member to. Only communities to which the contact has previouly accepted the invitation to join, or has pending invitations are returned.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getCommunities" method="get" path="/self-service/v2/contacts/{id}/communities" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetCommunities({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    includeTotal: true,
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceGetCommunities } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-communities.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetCommunities(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    includeTotal: true,
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetCommunities failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetCommunitiesRequest](../../models/operations/com-crm-contact-self-service-resource-get-communities-request.md)                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetCommunitiesResponse](../../models/operations/com-crm-contact-self-service-resource-get-communities-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceLeaveCommunity

Leave from a contact community

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_leaveCommunity" method="delete" path="/self-service/v2/contacts/{id}/communities/{community_owner_id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  await crmcom.communities.comCrmContactSelfServiceResourceLeaveCommunity({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    communityOwnerId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    id: "5096c4d4-c387-9888-d631-80e74546e2db",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceLeaveCommunity } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-leave-community.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceLeaveCommunity(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    communityOwnerId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
    id: "5096c4d4-c387-9888-d631-80e74546e2db",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceLeaveCommunity failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceLeaveCommunityRequest](../../models/operations/com-crm-contact-self-service-resource-leave-community-request.md)                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceLeaveCommunitySecurity](../../models/operations/com-crm-contact-self-service-resource-leave-community-security.md)                 | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceListContactGroups

Lists all groups that a contact has created

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_listContactGroups" method="get" path="/self-service/v2/contacts/{id}/groups" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceListContactGroups({
    id: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceListContactGroups } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-list-contact-groups.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceListContactGroups(crmcom, {
    id: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceListContactGroups failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceListContactGroupsRequest](../../models/operations/com-crm-contact-self-service-resource-list-contact-groups-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceListContactGroupsResponse](../../models/operations/com-crm-contact-self-service-resource-list-contact-groups-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceUpdateContactGroupName

Update a contact group name

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_updateContactGroupName" method="put" path="/self-service/v2/contacts/{id}/groups/{name}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceUpdateContactGroupName({
    id: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    name: "Family",
    body: {
      name: "Cousins",
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
import { communitiesComCrmContactSelfServiceResourceUpdateContactGroupName } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-update-contact-group-name.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceUpdateContactGroupName(crmcom, {
    id: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    name: "Family",
    body: {
      name: "Cousins",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceUpdateContactGroupName failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceUpdateContactGroupNameRequest](../../models/operations/com-crm-contact-self-service-resource-update-contact-group-name-request.md) | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceUpdateContactGroupNameResponse](../../models/operations/com-crm-contact-self-service-resource-update-contact-group-name-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceListContactRelationship

Lists all people that a contact's community has. The Web API returns only community people who accepted the invitation to join the community.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_listContactRelationship" method="get" path="/self-service/v2/contacts/{id}/people" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceListContactRelationship({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    group: "Employees",
    includeTotal: true,
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceListContactRelationship } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-list-contact-relationship.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceListContactRelationship(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    group: "Employees",
    includeTotal: true,
    sort: "CREATED_DATE,UPDATED_DATE,NAME,SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceListContactRelationship failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                       | Type                                                                                                                                                                            | Required                                                                                                                                                                        | Description                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceListContactRelationshipRequest](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-request.md) | :heavy_check_mark:                                                                                                                                                              | The request object to use for the request.                                                                                                                                      |
| `options`                                                                                                                                                                       | RequestOptions                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                              | Used to set various options for making HTTP requests.                                                                                                                           |
| `options.fetchOptions`                                                                                                                                                          | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                         | :heavy_minus_sign:                                                                                                                                                              | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.  |
| `options.retries`                                                                                                                                                               | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                              | Enables retrying HTTP requests under certain failure conditions.                                                                                                                |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceListContactRelationshipResponse](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceAddContactRelationship

Add a new person to a contact's community. The new community person can either be an existing contact or even a contact who is not yet registered. In both cases only Contacts of type Person can be included in the community. In addition, the contact that adds new community people must have the appropriate permissions to do so.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_addContactRelationship" method="post" path="/self-service/v2/contacts/{id}/people" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceAddContactRelationship({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    body: {
      email: "johndoe@crm.com",
      phone: {
        countryCode: "CYP",
        number: "99123456",
      },
      relationId: "ce27a6f8-bb1c-ee1a-d0ab-292ba154d8e4",
      isAdmin: true,
      permissions: [
        "CONTACT_MANAGEMENT",
      ],
      devices: [
        "123e4567-e89b-12d3-a456-426614174000",
        "987f6543-e21a-34c5-b678-123456789abc",
        "456a7890-b12c-34d5-f678-abcdef123456",
      ],
      walletSharing: {
        isEnabled: true,
        commercePools: [
          "e97129fb-94e8-fbbf-b35c-6b4b3645a25b",
        ],
        method: "AUTO",
        maxAmount: 50,
      },
      contact: {
        firstName: "John",
        lastName: "Doe",
        phone: {
          countryCode: "CYP",
          number: "99123456",
        },
      },
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
import { communitiesComCrmContactSelfServiceResourceAddContactRelationship } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-add-contact-relationship.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceAddContactRelationship(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    body: {
      email: "johndoe@crm.com",
      phone: {
        countryCode: "CYP",
        number: "99123456",
      },
      relationId: "ce27a6f8-bb1c-ee1a-d0ab-292ba154d8e4",
      isAdmin: true,
      permissions: [
        "CONTACT_MANAGEMENT",
      ],
      devices: [
        "123e4567-e89b-12d3-a456-426614174000",
        "987f6543-e21a-34c5-b678-123456789abc",
        "456a7890-b12c-34d5-f678-abcdef123456",
      ],
      walletSharing: {
        isEnabled: true,
        commercePools: [
          "e97129fb-94e8-fbbf-b35c-6b4b3645a25b",
        ],
        method: "AUTO",
        maxAmount: 50,
      },
      contact: {
        firstName: "John",
        lastName: "Doe",
        phone: {
          countryCode: "CYP",
          number: "99123456",
        },
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceAddContactRelationship failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceAddContactRelationshipRequest](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-request.md)  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceAddContactRelationshipResponse](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetContactRelationship

Retrieve an existing person from a contact's community. Web API returns detailed information of a contact that accepted the invitation to join a Community.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactRelationship" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactRelationship({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceGetContactRelationship } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-relationship.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactRelationship(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactRelationship failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipRequest](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-request.md)  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetContactRelationshipResponse](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceUpdateContactRelationship

Update an existing person in a contact's community. The Web API is successful only if the contact perfoming the update has the required permissions to do it or if it's the owner of the community.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_updateContactRelationship" method="put" path="/self-service/v2/contacts/{id}/people/{relationship_id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceUpdateContactRelationship({
    id: "41531d41-2a77-fc41-5643-d84dfbefc1ff",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    body: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      relationId: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
      group: "Family",
      isAdmin: true,
      walletSharing: {
        isEnabled: true,
        method: "AUTO",
        maxAmount: 50,
      },
      termedTransfer: {
        active: true,
        amount: 100,
        currencyCode: "EUR",
        commercePoolId: "cf4e4bb3-1f10-4f26-a675-db8f3c0a891f",
        schedule: {
          frequency: "MONTHLY",
          dayOfWeek: "MONDAY",
          dayOfMonth: 15,
        },
      },
      usageAllowance: {
        organisations: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          },
        ],
      },
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
import { communitiesComCrmContactSelfServiceResourceUpdateContactRelationship } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-update-contact-relationship.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceUpdateContactRelationship(crmcom, {
    id: "41531d41-2a77-fc41-5643-d84dfbefc1ff",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    body: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      relationId: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
      group: "Family",
      isAdmin: true,
      walletSharing: {
        isEnabled: true,
        method: "AUTO",
        maxAmount: 50,
      },
      termedTransfer: {
        active: true,
        amount: 100,
        currencyCode: "EUR",
        commercePoolId: "cf4e4bb3-1f10-4f26-a675-db8f3c0a891f",
        schedule: {
          frequency: "MONTHLY",
          dayOfWeek: "MONDAY",
          dayOfMonth: 15,
        },
      },
      usageAllowance: {
        organisations: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          },
        ],
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceUpdateContactRelationship failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                           | Type                                                                                                                                                                                | Required                                                                                                                                                                            | Description                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceUpdateContactRelationshipRequest](../../models/operations/com-crm-contact-self-service-resource-update-contact-relationship-request.md) | :heavy_check_mark:                                                                                                                                                                  | The request object to use for the request.                                                                                                                                          |
| `options`                                                                                                                                                                           | RequestOptions                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                  | Used to set various options for making HTTP requests.                                                                                                                               |
| `options.fetchOptions`                                                                                                                                                              | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                             | :heavy_minus_sign:                                                                                                                                                                  | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.      |
| `options.retries`                                                                                                                                                                   | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                  | Enables retrying HTTP requests under certain failure conditions.                                                                                                                    |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceUpdateContactRelationshipResponse](../../models/operations/com-crm-contact-self-service-resource-update-contact-relationship-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceRemoveContactRelationship

Delete an existing person from a contact’s community

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_removeContactRelationship" method="delete" path="/self-service/v2/contacts/{id}/people/{relationship_id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.communities.comCrmContactSelfServiceResourceRemoveContactRelationship({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    relationshipId: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { communitiesComCrmContactSelfServiceResourceRemoveContactRelationship } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-remove-contact-relationship.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceRemoveContactRelationship(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    relationshipId: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceRemoveContactRelationship failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                           | Type                                                                                                                                                                                | Required                                                                                                                                                                            | Description                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceRemoveContactRelationshipRequest](../../models/operations/com-crm-contact-self-service-resource-remove-contact-relationship-request.md) | :heavy_check_mark:                                                                                                                                                                  | The request object to use for the request.                                                                                                                                          |
| `options`                                                                                                                                                                           | RequestOptions                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                  | Used to set various options for making HTTP requests.                                                                                                                               |
| `options.fetchOptions`                                                                                                                                                              | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                             | :heavy_minus_sign:                                                                                                                                                                  | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.      |
| `options.retries`                                                                                                                                                                   | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                  | Enables retrying HTTP requests under certain failure conditions.                                                                                                                    |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetContactPersonAllowance

Returns a community member’s usage allowance for a set of products (SKUs, types, families and categories).

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonAllowance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                            | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                            | [operations.ComCrmContactSelfServiceResourceGetContactPersonAllowanceRequest](../../models/operations/com-crm-contact-self-service-resource-get-contact-person-allowance-request.md) | :heavy_check_mark:                                                                                                                                                                   | The request object to use for the request.                                                                                                                                           |
| `options`                                                                                                                                                                            | RequestOptions                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                   | Used to set various options for making HTTP requests.                                                                                                                                |
| `options.fetchOptions`                                                                                                                                                               | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                              | :heavy_minus_sign:                                                                                                                                                                   | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.       |
| `options.retries`                                                                                                                                                                    | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                   | Enables retrying HTTP requests under certain failure conditions.                                                                                                                     |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetContactPersonAllowanceResponse](../../models/operations/com-crm-contact-self-service-resource-get-contact-person-allowance-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceAddContactRelationshipProductAllowance

Add product allowance to a contact's community person.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_addContactRelationshipProductAllowance" method="post" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceAddContactRelationshipProductAllowance({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    body: {
      productsAllowance: [
        {
          groupId: "string",
          itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
          cashLimits: {
            perTransaction: 0,
            perDay: 0,
            perBillingCycle: 0,
          },
          usageLimits: {
            perTransaction: 0,
            perDay: 0,
            perBillingCycle: 0,
          },
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
import {
  communitiesComCrmContactSelfServiceResourceAddContactRelationshipProductAllowance,
} from "crmcom/funcs/communities-com-crm-contact-self-service-resource-add-contact-relationship-product-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceAddContactRelationshipProductAllowance(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    body: {
      productsAllowance: [
        {
          groupId: "string",
          itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
          cashLimits: {
            perTransaction: 0,
            perDay: 0,
            perBillingCycle: 0,
          },
          usageLimits: {
            perTransaction: 0,
            perDay: 0,
            perBillingCycle: 0,
          },
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceAddContactRelationshipProductAllowance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                       | Type                                                                                                                                                                                                            | Required                                                                                                                                                                                                        | Description                                                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceAddContactRelationshipProductAllowanceRequest](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-product-allowance-request.md) | :heavy_check_mark:                                                                                                                                                                                              | The request object to use for the request.                                                                                                                                                                      |
| `options`                                                                                                                                                                                                       | RequestOptions                                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                                              | Used to set various options for making HTTP requests.                                                                                                                                                           |
| `options.fetchOptions`                                                                                                                                                                                          | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                              | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                  |
| `options.retries`                                                                                                                                                                                               | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                              | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceAddContactRelationshipProductAllowanceResponse](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-product-allowance-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance

Updates and existing person allowance product

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_updateContactRelationshipProductAllowance" method="put" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance/{product_allowance_id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.communities.comCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    productAllowanceId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    body: {
      groupId: "string",
      itemType: "PRODUCT",
      itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      cashLimits: {
        perTransaction: 0,
        perDay: 0,
        perBillingCycle: 0,
      },
      usageLimits: {
        perTransaction: 0,
        perDay: 0,
        perBillingCycle: 0,
      },
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  communitiesComCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance,
} from "crmcom/funcs/communities-com-crm-contact-self-service-resource-update-contact-relationship-product-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    productAllowanceId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    body: {
      groupId: "string",
      itemType: "PRODUCT",
      itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      cashLimits: {
        perTransaction: 0,
        perDay: 0,
        perBillingCycle: 0,
      },
      usageLimits: {
        perTransaction: 0,
        perDay: 0,
        perBillingCycle: 0,
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                             | Type                                                                                                                                                                                                                  | Required                                                                                                                                                                                                              | Description                                                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceUpdateContactRelationshipProductAllowanceRequest](../../models/operations/com-crm-contact-self-service-resource-update-contact-relationship-product-allowance-request.md) | :heavy_check_mark:                                                                                                                                                                                                    | The request object to use for the request.                                                                                                                                                                            |
| `options`                                                                                                                                                                                                             | RequestOptions                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                    | Used to set various options for making HTTP requests.                                                                                                                                                                 |
| `options.fetchOptions`                                                                                                                                                                                                | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                                    | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                        |
| `options.retries`                                                                                                                                                                                                     | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                    | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                      |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance

Delete an existing allowance product from a contact’s community

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_removeContactRelationshipProductAllowance" method="delete" path="/self-service/v2/contacts/{id}/people/{relationship_id}/products_allowance/{product_allowance_id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.communities.comCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance({
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    productAllowanceId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  communitiesComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance,
} from "crmcom/funcs/communities-com-crm-contact-self-service-resource-remove-contact-relationship-product-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance(crmcom, {
    id: "3afad71d-e015-4e98-a464-f438c93edcde",
    productAllowanceId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                             | Type                                                                                                                                                                                                                  | Required                                                                                                                                                                                                              | Description                                                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowanceRequest](../../models/operations/com-crm-contact-self-service-resource-remove-contact-relationship-product-allowance-request.md) | :heavy_check_mark:                                                                                                                                                                                                    | The request object to use for the request.                                                                                                                                                                            |
| `options`                                                                                                                                                                                                             | RequestOptions                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                    | Used to set various options for making HTTP requests.                                                                                                                                                                 |
| `options.fetchOptions`                                                                                                                                                                                                | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                                    | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                        |
| `options.retries`                                                                                                                                                                                                     | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                    | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                      |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance

Returns a community member’s remaining usage allowance for a set of products (SKUs, types, families and categories).

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonRemainingAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/remaining_products_allowance" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-remaining-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonRemainingAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/remaining_products_allowance" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-remaining-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonRemainingAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/remaining_products_allowance" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-remaining-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonRemainingAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/remaining_products_allowance" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-remaining-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getContactPersonRemainingAllowance" method="get" path="/self-service/v2/contacts/{id}/people/{relationship_id}/remaining_products_allowance" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.communities.comCrmContactSelfServiceResourceGetContactPersonRemainingAllowance({
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
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
import { communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance } from "crmcom/funcs/communities-com-crm-contact-self-service-resource-get-contact-person-remaining-allowance.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance(crmcom, {
    id: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
    relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("communitiesComCrmContactSelfServiceResourceGetContactPersonRemainingAllowance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                               | Type                                                                                                                                                                                                    | Required                                                                                                                                                                                                | Description                                                                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                               | [operations.ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowanceRequest](../../models/operations/com-crm-contact-self-service-resource-get-contact-person-remaining-allowance-request.md) | :heavy_check_mark:                                                                                                                                                                                      | The request object to use for the request.                                                                                                                                                              |
| `options`                                                                                                                                                                                               | RequestOptions                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                      | Used to set various options for making HTTP requests.                                                                                                                                                   |
| `options.fetchOptions`                                                                                                                                                                                  | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                      | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                          |
| `options.retries`                                                                                                                                                                                       | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                      | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                        |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowanceResponse](../../models/operations/com-crm-contact-self-service-resource-get-contact-person-remaining-allowance-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |