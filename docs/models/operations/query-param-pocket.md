# QueryParamPocket

Filter transactions by pocket: CRM.COM = CRM.COM pocket, BUSINESS = business open pocket, BUSINESS_COMMERCE = business commerce pocket. If not specified then transactions for all business pockets are retrieved.

## Example Usage

```typescript
import { QueryParamPocket } from "crm/models/operations";

let value: QueryParamPocket = "CRMCOM";
```

## Values

```typescript
"CRMCOM" | "BUSINESS" | "BUSINESS_COMMERCE"
```