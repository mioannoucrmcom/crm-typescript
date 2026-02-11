# Features

Details about the features that will be supported by the app

## Example Usage

```typescript
import { Features } from "crmcom/models/operations";

let value: Features = {
  contact: {
    contact: {
      walletCodeFormat: "BARCODE",
      profile: [
        {
          isSupported: true,
        },
      ],
      communities: {
        isSupported: true,
      },
      countryCallingCodes: [
        {
          country: "CYP",
        },
      ],
      preferredLanguageCode: "EN",
    },
    businessNetwork: {
      isSupported: true,
      multitenancy: {
        isSupported: true,
      },
    },
    crm: {
      isSupported: true,
      serviceRequests: {
        isSupported: true,
      },
    },
    finance: {
      isSupported: true,
      walletTopUp: true,
      topUpCommercePools: [
        {
          id: "dc01f65b-a482-48f1-9fda-c163df72f28f",
          name: "Redeem Anywhere",
          description: "Ability to redeem on any organisation/day/product",
        },
      ],
      walletPayout: true,
      redeemPass: {
        isSupported: true,
      },
      transfer: {
        commercePools: [
          {
            id: "dc01f65b-a482-48f1-9fda-c163df72f28f",
            name: "Redeem Anywhere",
            description: "Ability to redeem on any organisation/day/product",
          },
        ],
      },
      topupAmounts: [
        {
          currencyCode: "EUR",
          amounts: [
            10,
            20,
            50,
            100,
          ],
        },
      ],
      redeemMethod: "ON_REQUEST, AUTOMATIC, ON_SPEND",
      egiftsEnabled: true,
      autoTopupEnabled: true,
    },
    order: {
      isSupported: true,
      pickUp: {
        isSupported: true,
        queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
        queueName: "Default queue",
      },
      delivery: {
        isSupported: true,
        queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
        queueName: "Default queue",
      },
      directSale: {
        isSupported: true,
        queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
        queueName: "Default Queue",
      },
      preferredOrganisation: true,
      orderCatalogues: [
        {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
      ],
      useWalletFunds: {
        specificFundsAmount: false,
        coverFullBasket: false,
      },
      fulfilmentFlows: {
        fulfilmentFlow: "SINGLE_MERCHANT",
        allowDeliverySelection: true,
      },
      supportProductAdditionalNotes: true,
    },
    reward: {
      tiering: true,
      preferredOrganisation: true,
      referFriend: {
        isSupported: true,
      },
      otpSpend: {
        isSupported: true,
        codeFormat: "BARCODE",
        spendAttributes: [
          {
            type: "AMOUNT",
          },
        ],
      },
      selfSubmitPurchases: {
        isSupported: true,
        selfSubmitMethods: [
          "BARCODE",
        ],
      },
    },
    marketing: {
      isSupported: true,
      embeddedLinks: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          title: "News & upcoming event",
          url: "https://www.guababeachbar.com/news&events",
          sortOrder: 1,
          languageCode: "EN",
          creatives: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              width: 2159,
              height: 3075,
              format: "jpg",
              url: "https://assets.crm.com/image/offer.jpg",
              publicId: "crm-com/image",
              media: [
                {
                  width: 200,
                  height: 300,
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
    },
    shortcuts: {
      shortcuts: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          sortOrder: 5,
          type: "TOP_UP_WALLET",
          label: "Report a problem",
          languageCode: "EN",
          creatives: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              width: 2159,
              height: 3075,
              format: "jpg",
              url: "https://assets.crm.com/image/offer.jpg",
              publicId: "crm-com/image",
              media: [
                {
                  width: 200,
                  height: 300,
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
    },
    mobilePass: {
      isSupported: true,
    },
  },
  merchant: {
    purchase: {
      manualSpend: true,
      automaticSpend: true,
      spendFullPurchaseAmount: true,
      restrictFullyCovered: true,
    },
  },
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `contact`                                                                 | [operations.FeaturesContact](../../models/operations/features-contact.md) | :heavy_minus_sign:                                                        | The contact features that will be supported by the application            |
| `merchant`                                                                | [operations.Merchant](../../models/operations/merchant.md)                | :heavy_minus_sign:                                                        | The merchant features that will be supported by the application           |