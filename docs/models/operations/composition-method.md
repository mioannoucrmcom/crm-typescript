# CompositionMethod

Product Composition

## Example Usage

```typescript
import { CompositionMethod } from "crmcom/models/operations";

let value: CompositionMethod = "FIXED_BUNDLE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "FLEXIBLE_BUNDLE" | "FIXED_BUNDLE" | "COMPOSITE" | Unrecognized<string>
```