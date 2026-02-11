# PocketResponse

Specifies which pocket the transaction was logged against. CRMCOM = CRM.COM pocket, BUSINESS = business open pocket, BUSINESS_COMMERCE = business commerce pocket

## Example Usage

```typescript
import { PocketResponse } from "crmcom/models/operations";

let value: PocketResponse = "BUSINESS_COMMERCE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"CRMCOM" | "BUSINESS" | "BUSINESS_COMMERCE" | Unrecognized<string>
```