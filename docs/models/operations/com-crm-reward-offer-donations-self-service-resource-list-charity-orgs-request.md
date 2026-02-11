# ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsRequest

## Example Usage

```typescript
import { ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsRequest } from "crm/models/operations";

let value: ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsRequest =
  {
    includeCreatives: true,
  };
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   | Example                                                                       |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `includeCreatives`                                                            | *boolean*                                                                     | :heavy_minus_sign:                                                            | Determines whether creatives will also be returned or not. Defaults to false. | true                                                                          |
| `type`                                                                        | *string*                                                                      | :heavy_minus_sign:                                                            | Search organisations based on Donation offer types                            |                                                                               |