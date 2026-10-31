# RedeemMethod

Defines which redeem methods are allowed

## Example Usage

```typescript
import { RedeemMethod } from "crm/models/operations";

let value: RedeemMethod = "DEFERRED";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"DEFERRED" | "INSTANT" | Unrecognized<string>
```