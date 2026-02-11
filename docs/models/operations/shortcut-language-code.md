# ShortcutLanguageCode

2-character language code based on ISO 639-1

## Example Usage

```typescript
import { ShortcutLanguageCode } from "crmcom/models/operations";

let value: ShortcutLanguageCode = "EN";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"EN" | "GR" | Unrecognized<string>
```