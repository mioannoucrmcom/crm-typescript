# CrossSellMeasurementUnit

Applicable only for Usage service to show the unit per which the price is applied

## Example Usage

```typescript
import { CrossSellMeasurementUnit } from "crm/models/operations";

let value: CrossSellMeasurementUnit = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Gigabytes",
  displayName: "GB",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0 |
| `name`                               | *string*                             | :heavy_minus_sign:                   | Measurement unit name                | Gigabytes                            |
| `displayName`                        | *string*                             | :heavy_minus_sign:                   | Measurement unit display name        | GB                                   |