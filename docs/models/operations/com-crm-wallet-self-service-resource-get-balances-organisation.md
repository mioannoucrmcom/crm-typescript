# ComCrmWalletSelfServiceResourceGetBalancesOrganisation

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetBalancesOrganisation } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetBalancesOrganisation = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Cafe",
  type: "MERCHANT",
  locations: [
    {
      name: "Head Office",
      addressLine1: "Elia Papakyriakou 21",
      addressLine2: "7 Stars Tower",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2415",
      countryCode: "CYP",
      lat: 35.157115,
      lon: 33.313719,
      googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                    | Type                                                                                                                                                     | Required                                                                                                                                                 | Description                                                                                                                                              | Example                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                     | *string*                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                       | The entity identifier                                                                                                                                    | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                     |
| `name`                                                                                                                                                   | *string*                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                       | The organisation name                                                                                                                                    | Cafe                                                                                                                                                     |
| `type`                                                                                                                                                   | [operations.ComCrmWalletSelfServiceResourceGetBalancesType](../../models/operations/com-crm-wallet-self-service-resource-get-balances-type.md)           | :heavy_minus_sign:                                                                                                                                       | The organisation type                                                                                                                                    | MERCHANT                                                                                                                                                 |
| `locations`                                                                                                                                              | [operations.ComCrmWalletSelfServiceResourceGetBalancesLocation](../../models/operations/com-crm-wallet-self-service-resource-get-balances-location.md)[] | :heavy_minus_sign:                                                                                                                                       | The locations of the organisation                                                                                                                        |                                                                                                                                                          |