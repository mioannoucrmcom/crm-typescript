# RedeemMethod

Defines which redeem methods are allowed

## Example Usage

```typescript
import { RedeemMethod } from "crmcom/models/operations";

let value: RedeemMethod = "DEFERRED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DEFERRED" | "INSTANT" | Unrecognized<string>
```