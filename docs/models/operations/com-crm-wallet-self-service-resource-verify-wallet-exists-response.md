# ComCrmWalletSelfServiceResourceVerifyWalletExistsResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceVerifyWalletExistsResponse } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceVerifyWalletExistsResponse = {
  walletExists: true,
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              | Example                                                                                  |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `walletExists`                                                                           | *boolean*                                                                                | :heavy_minus_sign:                                                                       | Indicates whether a wallet using the email or phone provided as identity, already exists | true                                                                                     |