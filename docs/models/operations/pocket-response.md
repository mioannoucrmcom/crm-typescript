# PocketResponse

Specifies which pocket the transaction was logged against. CRMCOM = CRM.COM pocket, BUSINESS = business open pocket, BUSINESS_COMMERCE = business commerce pocket

## Example Usage

```typescript
import { PocketResponse } from "crm/models/operations";

let value: PocketResponse = "BUSINESS_COMMERCE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"CRMCOM" | "BUSINESS" | "BUSINESS_COMMERCE" | Unrecognized<string>
```