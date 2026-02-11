# ValidityType

The validity type

## Example Usage

```typescript
import { ValidityType } from "crm/models/operations";

let value: ValidityType = "ALWAYS";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PERIOD" | "DATE" | "ALWAYS" | Unrecognized<string>
```