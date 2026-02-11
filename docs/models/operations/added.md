# Added

## Example Usage

```typescript
import { Added } from "crmcom/models/operations";

let value: Added = {
  productId: "2dc0809f-ed91-4b68-b912-5bd6064d901e",
  priceTermsId: "32c0809f-ed91-4b68-b912-5bd6064d901e",
};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                | Example                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `productId`                                                                                                                                | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The component service's identifier. Only termed services can eb specified and as ong as the service meets the bundle's allowed composition | 2dc0809f-ed91-4b68-b912-5bd6064d901e                                                                                                       |
| `priceTermsId`                                                                                                                             | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The component service's price terms                                                                                                        | 32c0809f-ed91-4b68-b912-5bd6064d901e                                                                                                       |