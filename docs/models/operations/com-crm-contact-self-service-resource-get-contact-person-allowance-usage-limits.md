# ComCrmContactSelfServiceResourceGetContactPersonAllowanceUsageLimits

Actual allowed and remaining usage (based on measurement units)

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactPersonAllowanceUsageLimits } from "crm/models/operations";

let value:
  ComCrmContactSelfServiceResourceGetContactPersonAllowanceUsageLimits = {};
```

## Fields

| Field                       | Type                        | Required                    | Description                 |
| --------------------------- | --------------------------- | --------------------------- | --------------------------- |
| `perTransaction`            | *number*                    | :heavy_minus_sign:          | Allowance per transaction   |
| `perDay`                    | *number*                    | :heavy_minus_sign:          | Allowance per day           |
| `perBillingCycle`           | *number*                    | :heavy_minus_sign:          | Allowance per billing cycle |