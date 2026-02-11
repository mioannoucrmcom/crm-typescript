# InformationType

The content type

## Example Usage

```typescript
import { InformationType } from "crm/models/operations";

let value: InformationType = "ABOUT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ABOUT" | "TERMS_CONDITIONS" | "PRIVACY_POLICY" | "FAQS" | Unrecognized<string>
```