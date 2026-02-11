# ChangeToService

Applicable and required when upgrading or downgrading a service

## Example Usage

```typescript
import { ChangeToService } from "crmcom/models/operations";

let value: ChangeToService = {
  productId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
  priceTermsId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
};
```

## Fields

| Field                                                                                                                                  | Type                                                                                                                                   | Required                                                                                                                               | Description                                                                                                                            | Example                                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| `productId`                                                                                                                            | *string*                                                                                                                               | :heavy_check_mark:                                                                                                                     | The new service product to which the service will be changed with                                                                      | 4dc0809f-ed91-4b68-b912-5bd6064d901e                                                                                                   |
| `priceTermsId`                                                                                                                         | *string*                                                                                                                               | :heavy_minus_sign:                                                                                                                     | Required when the new service has multiple price terms. If the new service product has a single price, then it will be used by default | 4dc0809f-ed91-4b68-b912-5bd6064d901e                                                                                                   |