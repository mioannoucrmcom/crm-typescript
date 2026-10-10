# CreditWalletBalance

The wallet balance to be credited when the pass is redeemed. For TOP_UP and GIFT passes only

## Example Usage

```typescript
import { CreditWalletBalance } from "crm/models/operations";

let value: CreditWalletBalance = "COMMERCE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"OPEN" | "COMMERCE" | Unrecognized<string>
```