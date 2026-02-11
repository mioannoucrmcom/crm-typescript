# Goal

The offer goal

## Example Usage

```typescript
import { Goal } from "crmcom/models/operations";

let value: Goal = "ACHIEVEMENT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ACHIEVEMENT" | "SPEND" | "VISITS" | "MEMBERSHIP" | Unrecognized<string>
```