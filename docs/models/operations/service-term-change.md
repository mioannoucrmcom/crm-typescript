# ServiceTermChange

## Example Usage

```typescript
import { ServiceTermChange } from "crm/models/operations";

let value: ServiceTermChange = {
  extendBy: {
    uot: "MINUTE",
  },
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `serviceId`                                                                            | *string*                                                                               | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `autoRenewalPreference`                                                                | [operations.AutoRenewalPreference](../../models/operations/auto-renewal-preference.md) | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `contractPreference`                                                                   | [operations.ContractPreference](../../models/operations/contract-preference.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `extendBy`                                                                             | [operations.ExtendBy](../../models/operations/extend-by.md)                            | :heavy_minus_sign:                                                                     | N/A                                                                                    |