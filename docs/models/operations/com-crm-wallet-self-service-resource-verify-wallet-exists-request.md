# ComCrmWalletSelfServiceResourceVerifyWalletExistsRequest

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceVerifyWalletExistsRequest } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceVerifyWalletExistsRequest = {
  type: "EMAIL",
  value: "99123456",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     | Example                                                                                         |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `type`                                                                                          | *string*                                                                                        | :heavy_minus_sign:                                                                              | A wallet can either be identified across the business network based on a phone or email address | EMAIL                                                                                           |
| `value`                                                                                         | *string*                                                                                        | :heavy_minus_sign:                                                                              | The wallet identity phone or email address depending on the identity's type                     | 99123456                                                                                        |