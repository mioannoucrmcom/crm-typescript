# SpendMethod

Define how awards can be/were spent (for SPEND transactions only)
 * `INSTANT` - Instant Discount
 * `AUTOMATIC_SPEND` - Automatic Spend Requests
 * `ON_REQUEST` - Spend on Customer Request


## Example Usage

```typescript
import { SpendMethod } from "crm/models/operations";

let value: SpendMethod = "INSTANT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ON_REQUEST" | "INSTANT" | "DEFERRED" | "AUTO_SPEND" | "VOUCHER" | Unrecognized<string>
```