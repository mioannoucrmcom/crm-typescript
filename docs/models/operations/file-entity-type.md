# FileEntityType

The file being uploaded is for this entity. The following types will be automatically deleted from the system after 1 week: ACCOUNT_STATEMENTS, INSIGHTS, REPORTS, SEGMENT_CONTACTS, PASSES.

## Example Usage

```typescript
import { FileEntityType } from "crm/models/operations";

let value: FileEntityType = "ORDERS";
```

## Values

```typescript
"CONTACTS" | "ORDERS" | "LEADS" | "SERVICE_REQUESTS" | "IMPORTS" | "IMPORTS_ERROR" | "ACCOUNT_STATEMENTS" | "INSIGHTS" | "REPORTS" | "SEGMENT_CONTACTS" | "PASSES" | "OTHER"
```