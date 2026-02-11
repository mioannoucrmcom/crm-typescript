# Billing

Latest billing information of the service

## Example Usage

```typescript
import { Billing } from "crmcom/models/operations";

let value: Billing = {
  billedFrom: 1625555027,
  billedTo: 1625555027,
};
```

## Fields

| Field                   | Type                    | Required                | Description             | Example                 |
| ----------------------- | ----------------------- | ----------------------- | ----------------------- | ----------------------- |
| `billedFrom`            | *number*                | :heavy_minus_sign:      | Latest billed from date | 1625555027              |
| `billedTo`              | *number*                | :heavy_minus_sign:      | Billed up to date       | 1625555027              |