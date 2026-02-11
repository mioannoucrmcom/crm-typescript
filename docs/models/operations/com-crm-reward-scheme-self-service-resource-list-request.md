# ComCrmRewardSchemeSelfServiceResourceListRequest

## Example Usage

```typescript
import { ComCrmRewardSchemeSelfServiceResourceListRequest } from "crm/models/operations";

let value: ComCrmRewardSchemeSelfServiceResourceListRequest = {
  isSigned: true,
  name: "CRMdotCOM Reward Scheme",
};
```

## Fields

| Field                                                | Type                                                 | Required                                             | Description                                          | Example                                              |
| ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| `isSigned`                                           | *boolean*                                            | :heavy_minus_sign:                                   | Filter based on whether contact has signed up or not | true                                                 |
| `name`                                               | *string*                                             | :heavy_minus_sign:                                   | Filter based on reward scheme name                   | CRMdotCOM Reward Scheme                              |