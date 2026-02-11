# Field

The custom field’s UI field type

## Example Usage

```typescript
import { Field } from "crm/models/operations";

let value: Field = "CHECKBOX";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SINGLE_LINE" | "MULTIPLE_LINES" | "SELECTION" | "CHECKBOX" | "RADIO_BUTTONS" | "TIMESTAMP" | "DATE" | "NUMBER" | "AMOUNT" | "CONTENT" | "NUMBERING_SCHEME" | Unrecognized<string>
```