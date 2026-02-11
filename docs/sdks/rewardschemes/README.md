# RewardSchemes

## Overview

Reward Schemes

### Available Operations

* [comCrmRewardSchemeSelfServiceResourceList](#comcrmrewardschemeselfserviceresourcelist) - Search Reward Schemes

## comCrmRewardSchemeSelfServiceResourceList

Retrieve all active reward schemes

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.RewardSchemeSelfServiceResource_list" method="get" path="/self-service/v2/reward_schemes" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.rewardSchemes.comCrmRewardSchemeSelfServiceResourceList({
    isSigned: true,
    name: "CRMdotCOM Reward Scheme",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { rewardSchemesComCrmRewardSchemeSelfServiceResourceList } from "crm/funcs/reward-schemes-com-crm-reward-scheme-self-service-resource-list.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await rewardSchemesComCrmRewardSchemeSelfServiceResourceList(crm, {
    isSigned: true,
    name: "CRMdotCOM Reward Scheme",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("rewardSchemesComCrmRewardSchemeSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmRewardSchemeSelfServiceResourceListRequest](../../models/operations/com-crm-reward-scheme-self-service-resource-list-request.md)                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmRewardSchemeSelfServiceResourceListResponse](../../models/operations/com-crm-reward-scheme-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |