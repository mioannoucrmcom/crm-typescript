# Urgency

The default urgent level

## Example Usage

```typescript
import { Urgency } from "crm/models/operations";

let value: Urgency = "MEDIUM";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"HIGH" | "MEDIUM" | "LOW" | Unrecognized<string>
```