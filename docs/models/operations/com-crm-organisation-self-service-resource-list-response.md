# ComCrmOrganisationSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmOrganisationSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmOrganisationSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Delicious Bite",
      description: "Lorem Ipsum",
      industryName: "Restaurant",
      industrySectors: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Bar",
          relatedIndustries: [
            {
              id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
              name: "Universal Name",
            },
          ],
        },
      ],
      businessActivities: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Bar & Grill",
        },
      ],
      addresses: [
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
        },
      ],
      tags: [
        {
          name: "Accounting",
        },
      ],
      contactInfo: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Main Office",
          value: "johndoe@deliciousfood.com",
          countryCode: "CYP",
        },
      ],
      operationDetails: {
        openingHours: [
          {
            dayOfWeek: "MONDAY",
            open: "09:00",
            close: "17:00",
            operation: "DELIVERY",
          },
        ],
        shortTermOperations: [
          {
            isClosed: false,
          },
        ],
      },
      contactRegistry: {},
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
      orderCatalogs: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          displayName: "Drinks Menu",
          timeAvailability: [
            {
              startTime: "09:00",
              endTime: "17:00",
            },
          ],
          supplyMethods: [
            "DELIVERY",
          ],
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
      wifiSites: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          siteId: "88quh2m6",
          integration: {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                               | Type                                                                                                                                                | Required                                                                                                                                            | Description                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                            | [operations.ComCrmOrganisationSelfServiceResourceListPaging](../../models/operations/com-crm-organisation-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                  | N/A                                                                                                                                                 |
| `content`                                                                                                                                           | [operations.ComCrmOrganisationSelfServiceResourceListContent](../../models/operations/com-crm-organisation-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                  | N/A                                                                                                                                                 |