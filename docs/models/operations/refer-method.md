# ReferMethod

## Example Usage

```typescript
import { ReferMethod } from "crm/models/operations";

let value: ReferMethod = "EMAIL";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"EMAIL" | "SMS" | Unrecognized<string>
```