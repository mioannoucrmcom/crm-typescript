# Field

The custom field’s UI field type

## Example Usage

```typescript
import { Field } from "crm/models/operations";

let value: Field = "CHECKBOX";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"SINGLE_LINE" | "MULTIPLE_LINES" | "SELECTION" | "CHECKBOX" | "RADIO_BUTTONS" | "TIMESTAMP" | "DATE" | "NUMBER" | "AMOUNT" | "CONTENT" | "NUMBERING_SCHEME" | Unrecognized<string>
```