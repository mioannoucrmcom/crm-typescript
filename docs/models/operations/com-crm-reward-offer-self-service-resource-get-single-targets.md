# ComCrmRewardOfferSelfServiceResourceGetSingleTargets

The targerted organisations that events performed on should be located at

## Example Usage

```typescript
import { ComCrmRewardOfferSelfServiceResourceGetSingleTargets } from "crm/models/operations";

let value: ComCrmRewardOfferSelfServiceResourceGetSingleTargets = {
  organisations: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Bravo Bakery",
      locations: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Head Office",
          addressLine1: "Elia Papakyriakou 21",
          addressLine2: "7 Tower Stars",
          stateProvinceCounty: "Egkomi",
          townCity: "Nicosia",
          postalCode: "2415",
          countryCode: "CYP",
          careOf: "c/o Company",
          lat: 35.157115,
          lon: 35.342115,
          googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
          isPrimary: true,
          isBilling: true,
          isTestMode: true,
        },
      ],
      type: "MERCHANT",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                   | Type                                                                                                                                                                    | Required                                                                                                                                                                | Description                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `organisations`                                                                                                                                                         | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleOrganisation](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-organisation.md)[] | :heavy_minus_sign:                                                                                                                                                      | The targerted organisations that events performed on should be located at                                                                                               |