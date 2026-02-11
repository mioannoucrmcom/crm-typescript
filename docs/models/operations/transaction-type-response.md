# TransactionTypeResponse

Types of financial transactions which can be performed against a contact's account or wallet

## Example Usage

```typescript
import { TransactionTypeResponse } from "crm/models/operations";

let value: TransactionTypeResponse = "INVOICE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"INVOICE" | "CREDIT_NOTE" | "PAYMENT" | "REFUND" | "PAYOUT" | "TOP_UP" | "TRANSFER" | "MANUAL_JOURNAL" | "SETTLEMENT_PROCESS" | Unrecognized<string>
```