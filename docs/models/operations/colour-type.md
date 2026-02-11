# ColourType

Defines the component on which the color will be applied

## Example Usage

```typescript
import { ColourType } from "crm/models/operations";

let value: ColourType = "PRIMARY_COLOUR";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"LANDING_BACKGROUND" | "LANDING_CARD" | "LANDING_TEXT" | "SCREEN_CARD" | "SCREEN_BUTTON" | "SCREEN_WALLET" | "LEGACY_BACKGROUND" | "LEGACY_BUTTON" | "LEGACY_CARD" | "PRIMARY_COLOUR" | "SECONDARY_COLOUR" | Unrecognized<string>
```