# Priority

The default priority level

## Example Usage

```typescript
import { Priority } from "crmcom/models/operations";

let value: Priority = "MEDIUM";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"URGENT" | "HIGH" | "MEDIUM" | "LOW" | Unrecognized<string>
```