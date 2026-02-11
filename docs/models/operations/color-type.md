# ColorType

The color

## Example Usage

```typescript
import { ColorType } from "crmcom/models/operations";

let value: ColorType = "BACKGROUND";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BACKGROUND" | "HEADER" | "BUTTON" | "TEXT" | "FOOTER" | "HEADER_TEXT" | "FOOTER_TEXT" | "BUTTON_TEXT" | Unrecognized<string>
```