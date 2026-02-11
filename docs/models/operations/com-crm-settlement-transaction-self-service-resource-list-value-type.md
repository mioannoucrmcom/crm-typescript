# ComCrmSettlementTransactionSelfServiceResourceListValueType

Defines whether the fee is amount or percentage based
 * `AMOUNT` - Fee will be amount based
 * `PERCENTAGE` - Fee will be percentage based


## Example Usage

```typescript
import { ComCrmSettlementTransactionSelfServiceResourceListValueType } from "crm/models/operations";

let value: ComCrmSettlementTransactionSelfServiceResourceListValueType =
  "AMOUNT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AMOUNT" | "PERCENTAGE" | Unrecognized<string>
```