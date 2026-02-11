# ComCrmEstimateSelfServiceResourceEstimateInvoicingPeriod

Invoiced period applicable only when invoicing a termed service.

## Example Usage

```typescript
import { ComCrmEstimateSelfServiceResourceEstimateInvoicingPeriod } from "crm/models/operations";

let value: ComCrmEstimateSelfServiceResourceEstimateInvoicingPeriod = {
  from: 1651172405,
  to: 1653764405,
};
```

## Fields

| Field                                                 | Type                                                  | Required                                              | Description                                           | Example                                               |
| ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| `from`                                                | *number*                                              | :heavy_minus_sign:                                    | The date from which the service is invoiced/credited  | 1651172405                                            |
| `to`                                                  | *number*                                              | :heavy_minus_sign:                                    | The date until which the service is invoiced/credited | 1653764405                                            |