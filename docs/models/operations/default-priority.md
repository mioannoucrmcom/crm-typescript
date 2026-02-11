# DefaultPriority

The queue’s default priority

## Example Usage

```typescript
import { DefaultPriority } from "crm/models/operations";

let value: DefaultPriority = {
  urgency: "MEDIUM",
  impact: "MEDIUM",
  priority: "MEDIUM",
};
```

## Fields

| Field                                                      | Type                                                       | Required                                                   | Description                                                | Example                                                    |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| `urgency`                                                  | [operations.Urgency](../../models/operations/urgency.md)   | :heavy_minus_sign:                                         | The default urgent level                                   | MEDIUM                                                     |
| `impact`                                                   | [operations.Impact](../../models/operations/impact.md)     | :heavy_minus_sign:                                         | The default impact level                                   | MEDIUM                                                     |
| `priority`                                                 | [operations.Priority](../../models/operations/priority.md) | :heavy_minus_sign:                                         | The default priority level                                 | MEDIUM                                                     |