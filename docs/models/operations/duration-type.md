# DurationType

Indicates whether the offering will be applied once, for a period of time or forever.

## Example Usage

```typescript
import { DurationType } from "crm/models/operations";

let value: DurationType = "PERIOD";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"ONE_TIME" | "FOREVER" | "PERIOD" | "VARIABLE_DISCOUNTS" | Unrecognized<string>
```