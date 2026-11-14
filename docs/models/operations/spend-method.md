# SpendMethod

Define how awards can be/were spent (for SPEND transactions only)
 * `INSTANT` - Instant Discount
 * `AUTOMATIC_SPEND` - Automatic Spend Requests
 * `ON_REQUEST` - Spend on Customer Request


## Example Usage

```typescript
import { SpendMethod } from "crm/models/operations";

let value: SpendMethod = "INSTANT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"ON_REQUEST" | "INSTANT" | "DEFERRED" | "AUTO_SPEND" | "VOUCHER" | Unrecognized<string>
```