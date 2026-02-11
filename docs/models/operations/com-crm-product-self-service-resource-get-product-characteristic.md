# ComCrmProductSelfServiceResourceGetProductCharacteristic

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductCharacteristic } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductCharacteristic = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  key: "colour",
  value: "RED",
  label: "RED",
  mandatory: true,
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                | Example                                                                                    |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `id`                                                                                       | *string*                                                                                   | :heavy_minus_sign:                                                                         | The entity identifier                                                                      | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                       |
| `key`                                                                                      | *string*                                                                                   | :heavy_minus_sign:                                                                         | Attribute’s key                                                                            | colour                                                                                     |
| `value`                                                                                    | *string*                                                                                   | :heavy_minus_sign:                                                                         | Attribute’s value                                                                          | RED                                                                                        |
| `label`                                                                                    | *string*                                                                                   | :heavy_minus_sign:                                                                         | Attribute’s label for UI purposes                                                          | RED                                                                                        |
| `mandatory`                                                                                | *boolean*                                                                                  | :heavy_minus_sign:                                                                         | Defines whether the attribute is mandatory (and cannot be removed from the product) or not | true                                                                                       |