# ComCrmApplicationSelfServiceResourceGetApplicationResponse

OK

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationResponse } from "crmcom/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Brew Coffee App",
  description: "Best coffee app",
  brandName: "Brew Coffee",
  appearance: {
    colours: [
      {
        value: "#eb4034",
      },
    ],
    darkMode: true,
  },
  information: {
    content: [
      {
        url: "https?/crm.com",
        richContent: "Terms & Conditions",
      },
    ],
    contactUs: {
      emailAddress: "info@crm.com",
      phone: {
        countryCode: "CYP",
        number: "22265566",
      },
      website: "https?/crm.com",
    },
  },
  features: {
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
  },
  platforms: [
    {
      platformId: "1762e052-4805-73eb-36f2-e77d6dc883e8",
      cloudName: "crmdotcom",
      version: "1.1",
    },
  ],
  authentication: {
    emailPassword: true,
    emailOtp: false,
    smsOtp: true,
    facebook: {
      isSupported: true,
      appId: "sfsdf-23-we-wer-3ew-dw",
    },
    demoContact: {
      isSupported: true,
      contact: {
        id: "76ee374d-cd38-4cde-9fa3-4eaa26e67a06",
        name: "John Doe",
      },
      otp: "123456",
    },
    guestContact: {
      isSupported: true,
      contact: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "John Doe",
      },
    },
    sso: {
      isSupported: true,
    },
  },
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
          url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
        },
      ],
      sortOrder: 5,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                                                                                             | Type                                                                                                                                                                                                                                                              | Required                                                                                                                                                                                                                                                          | Description                                                                                                                                                                                                                                                       | Example                                                                                                                                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                                                                              | *string*                                                                                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | The entity identifier                                                                                                                                                                                                                                             | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                                                                              |
| `name`                                                                                                                                                                                                                                                            | *string*                                                                                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | The application name                                                                                                                                                                                                                                              | Brew Coffee App                                                                                                                                                                                                                                                   |
| `description`                                                                                                                                                                                                                                                     | *string*                                                                                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | The application description                                                                                                                                                                                                                                       | Best coffee app                                                                                                                                                                                                                                                   |
| `brandName`                                                                                                                                                                                                                                                       | *string*                                                                                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | The business name shown in app front-end                                                                                                                                                                                                                          | Brew Coffee                                                                                                                                                                                                                                                       |
| `type`                                                                                                                                                                                                                                                            | [operations.ComCrmApplicationSelfServiceResourceGetApplicationType](../../models/operations/com-crm-application-self-service-resource-get-application-type.md)                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                                                                | The application type:<br/> * `NATIVE` - Mobile Consumer Applications (Apple and Google)<br/> * `NATIVE_MERCHANT` - Mobile Merchant Applications (Apple and Google)<br/> * `WEB` - Web Portal<br/> * `CAPTIVE` - Captive Portal<br/> * `CONSUMER_APP` - Consumer App (Portal and App)<br/> |                                                                                                                                                                                                                                                                   |
| `appearance`                                                                                                                                                                                                                                                      | [operations.Appearance](../../models/operations/appearance.md)                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                                                                | Details about the app appearance                                                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                   |
| `information`                                                                                                                                                                                                                                                     | [operations.Information](../../models/operations/information.md)                                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                                                                                                | Defines the app details (about, terms and conditions, privacy policy)                                                                                                                                                                                             |                                                                                                                                                                                                                                                                   |
| `features`                                                                                                                                                                                                                                                        | [operations.Features](../../models/operations/features.md)                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                                                                | Details about the features that will be supported by the app                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                   |
| `platforms`                                                                                                                                                                                                                                                       | [operations.ComCrmApplicationSelfServiceResourceGetApplicationPlatform](../../models/operations/com-crm-application-self-service-resource-get-application-platform.md)[]                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | Details about the application identifiers per supported platform                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                   |
| `authentication`                                                                                                                                                                                                                                                  | [operations.Authentication](../../models/operations/authentication.md)                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                                                                | Details on how customers can auth by the app                                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                   |
| `publicKey`                                                                                                                                                                                                                                                       | *string*                                                                                                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | N/A                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                   |
| `creatives`                                                                                                                                                                                                                                                       | [operations.ComCrmApplicationSelfServiceResourceGetApplicationCreative](../../models/operations/com-crm-application-self-service-resource-get-application-creative.md)[]                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                | Creatives images for marketing includes the primary image and scaled versions to create a srcset                                                                                                                                                                  |                                                                                                                                                                                                                                                                   |
| `firebaseConfig`                                                                                                                                                                                                                                                  | [operations.FirebaseConfig](../../models/operations/firebase-config.md)                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                                                                | N/A                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                   |
| `customizationConfig`                                                                                                                                                                                                                                             | [operations.CustomizationConfig](../../models/operations/customization-config.md)                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                                                                | N/A                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                   |
| `showRecommendations`                                                                                                                                                                                                                                             | *boolean*                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                | N/A                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                   |
| `showBestSelling`                                                                                                                                                                                                                                                 | *boolean*                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                | N/A                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                   |