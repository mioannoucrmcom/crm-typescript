# Colour

## Example Usage

```typescript
import { Colour } from "crmcom/models/operations";

let value: Colour = {
  value: "#eb4034",
};
```

## Fields

| Field                                                           | Type                                                            | Required                                                        | Description                                                     | Example                                                         |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `type`                                                          | [operations.ColourType](../../models/operations/colour-type.md) | :heavy_minus_sign:                                              | Defines the component on which the color will be applied        |                                                                 |
| `value`                                                         | *string*                                                        | :heavy_minus_sign:                                              | The color (hex) code                                            | #eb4034                                                         |