# TransactionTypeResponse

Types of financial transactions which can be performed against a contact's account or wallet

## Example Usage

```typescript
import { TransactionTypeResponse } from "crm/models/operations";

let value: TransactionTypeResponse = "INVOICE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"INVOICE" | "CREDIT_NOTE" | "PAYMENT" | "REFUND" | "PAYOUT" | "TOP_UP" | "TRANSFER" | "MANUAL_JOURNAL" | "SETTLEMENT_PROCESS" | Unrecognized<string>
```