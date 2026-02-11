# ServiceChangeType

## Example Usage

```typescript
import { ServiceChangeType } from "crmcom/models/operations";

let value: ServiceChangeType = "REMOVED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ADDED" | "REMOVED" | "UPDATED" | Unrecognized<string>
```