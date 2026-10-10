# ValueType

Will passes have a fixed or variable value? FIXED indicates that the pass value is predefined, VARIABLE allows the value of the pass to be set during creation (within a range of values)

## Example Usage

```typescript
import { ValueType } from "crm/models/operations";

let value: ValueType = "FIXED";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"FIXED" | "VARIABLE" | Unrecognized<string>
```