# ComCrmAccountSelfServiceResourceGetAccountJournalPeriod

Applicable only when the line item includes a termed service and denotes the invoiced/credited period

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceGetAccountJournalPeriod } from "crm/models/operations";

let value: ComCrmAccountSelfServiceResourceGetAccountJournalPeriod = {
  from: 1344242,
  to: 1344242,
};
```

## Fields

| Field              | Type               | Required           | Description        | Example            |
| ------------------ | ------------------ | ------------------ | ------------------ | ------------------ |
| `from`             | *number*           | :heavy_minus_sign: | Period start date  | 1344242            |
| `to`               | *number*           | :heavy_minus_sign: | Period end date    | 1344242            |