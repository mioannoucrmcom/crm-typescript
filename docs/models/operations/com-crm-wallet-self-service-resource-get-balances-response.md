# ComCrmWalletSelfServiceResourceGetBalancesResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetBalancesResponse } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceGetBalancesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Happy Hour",
      description:
        "Visit Coffee Shop any weekday early afternoon (3 to 5 pm) for happy hour",
      amount: 100.5,
      currencyCode: "EUR",
      expiration: {
        zeroToThirty: 30,
        thirtyToSixty: 50.5,
        sixtyToNinety: 55.5,
        ninetyPlus: 60,
      },
      organisations: [
        {
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
        },
      ],
      products: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Coffee",
          description: "Brazilian Coffee",
          sku: "COF-5541",
        },
      ],
      timings: [
        {
          day: 1,
          month: 10,
          startTime: "19:00",
          endTime: "21:00",
        },
      ],
      applicableForActivation: true,
      isActive: true,
      b2bDetails: {
        isPublished: true,
        isPromoted: true,
        promotedOrganisation: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                  | Type                                                                                                                                                   | Required                                                                                                                                               | Description                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `paging`                                                                                                                                               | [operations.ComCrmWalletSelfServiceResourceGetBalancesPaging](../../models/operations/com-crm-wallet-self-service-resource-get-balances-paging.md)     | :heavy_minus_sign:                                                                                                                                     | N/A                                                                                                                                                    |
| `content`                                                                                                                                              | [operations.ComCrmWalletSelfServiceResourceGetBalancesContent](../../models/operations/com-crm-wallet-self-service-resource-get-balances-content.md)[] | :heavy_minus_sign:                                                                                                                                     | N/A                                                                                                                                                    |