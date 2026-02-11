# ValueType

Will passes have a fixed or variable value? FIXED indicates that the pass value is predefined, VARIABLE allows the value of the pass to be set during creation (within a range of values)

## Example Usage

```typescript
import { ValueType } from "crmcom/models/operations";

let value: ValueType = "FIXED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FIXED" | "VARIABLE" | Unrecognized<string>
```