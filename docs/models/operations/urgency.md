# Urgency

The default urgent level

## Example Usage

```typescript
import { Urgency } from "crm/models/operations";

let value: Urgency = "MEDIUM";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"HIGH" | "MEDIUM" | "LOW" | Unrecognized<string>
```