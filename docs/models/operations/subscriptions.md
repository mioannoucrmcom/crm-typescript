# Subscriptions

Subscription settings for application

## Example Usage

```typescript
import { Subscriptions } from "crm/models/operations";

let value: Subscriptions = {};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `isSupported`                                                 | *boolean*                                                     | :heavy_minus_sign:                                            | Are subscriptions enabled?                                    |
| `actions`                                                     | [operations.Actions](../../models/operations/actions.md)      | :heavy_minus_sign:                                            | Subscription and service actions permitted by front-end users |