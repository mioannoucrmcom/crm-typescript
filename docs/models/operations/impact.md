# Impact

The default impact level

## Example Usage

```typescript
import { Impact } from "crmcom/models/operations";

let value: Impact = "MEDIUM";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"HIGH" | "MEDIUM" | "LOW" | Unrecognized<string>
```