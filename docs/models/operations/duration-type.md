# DurationType

Indicates whether the offering will be applied once, for a period of time or forever.

## Example Usage

```typescript
import { DurationType } from "crmcom/models/operations";

let value: DurationType = "PERIOD";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ONE_TIME" | "FOREVER" | "PERIOD" | "VARIABLE_DISCOUNTS" | Unrecognized<string>
```