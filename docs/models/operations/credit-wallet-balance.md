# CreditWalletBalance

The wallet balance to be credited when the pass is redeemed. For TOP_UP and GIFT passes only

## Example Usage

```typescript
import { CreditWalletBalance } from "crmcom/models/operations";

let value: CreditWalletBalance = "COMMERCE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"OPEN" | "COMMERCE" | Unrecognized<string>
```