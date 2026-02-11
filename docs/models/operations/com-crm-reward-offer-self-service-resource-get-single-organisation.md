# ComCrmRewardOfferSelfServiceResourceGetSingleOrganisation

## Example Usage

```typescript
import { ComCrmRewardOfferSelfServiceResourceGetSingleOrganisation } from "crmcom/models/operations";

let value: ComCrmRewardOfferSelfServiceResourceGetSingleOrganisation = {
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
};
```

## Fields

| Field                                                                                                                                                           | Type                                                                                                                                                            | Required                                                                                                                                                        | Description                                                                                                                                                     | Example                                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                            | *string*                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                              | The entity identifier                                                                                                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                            |
| `name`                                                                                                                                                          | *string*                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                              | The organisation name                                                                                                                                           | Bravo Bakery                                                                                                                                                    |
| `locations`                                                                                                                                                     | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleLocation](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-location.md)[] | :heavy_minus_sign:                                                                                                                                              | The organisation locations                                                                                                                                      |                                                                                                                                                                 |
| `type`                                                                                                                                                          | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleType](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-type.md)           | :heavy_minus_sign:                                                                                                                                              | The organisation type                                                                                                                                           | MERCHANT                                                                                                                                                        |