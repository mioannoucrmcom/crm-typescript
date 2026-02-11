# SpendBlocked

Details about whether the contact can spend or not

## Example Usage

```typescript
import { SpendBlocked } from "crm/models/operations";

let value: SpendBlocked = {
  date: 1583846865,
  status: true,
};
```

## Fields

| Field                                                  | Type                                                   | Required                                               | Description                                            | Example                                                |
| ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------------ |
| `date`                                                 | *number*                                               | :heavy_minus_sign:                                     | The date that the contact's spend blockage was updated | 1583846865                                             |
| `status`                                               | *boolean*                                              | :heavy_minus_sign:                                     | Defines whether the contact can spend or not           | true                                                   |