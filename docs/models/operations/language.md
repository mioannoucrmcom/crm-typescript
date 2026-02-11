# Language

## Example Usage

```typescript
import { Language } from "crmcom/models/operations";

let value: Language = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  language: "ENG",
};
```

## Fields

| Field                                                               | Type                                                                | Required                                                            | Description                                                         | Example                                                             |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `id`                                                                | *string*                                                            | :heavy_minus_sign:                                                  | The entity identifier that will be created                          | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                |
| `language`                                                          | [operations.LanguageEnum](../../models/operations/language-enum.md) | :heavy_minus_sign:                                                  | The supported glossary language code                                | ENG                                                                 |