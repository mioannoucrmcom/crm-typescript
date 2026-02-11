# ComCrmOrganisationSelfServiceResourceGetSingleResponse

OK

## Example Usage

```typescript
import { ComCrmOrganisationSelfServiceResourceGetSingleResponse } from "crmcom/models/operations";

let value: ComCrmOrganisationSelfServiceResourceGetSingleResponse = {
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
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
};
```

## Fields

| Field                                                                                                                                                                             | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       | Example                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                              | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The entity identifier                                                                                                                                                             | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                              |
| `name`                                                                                                                                                                            | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The organisation name                                                                                                                                                             | Delicious Bite                                                                                                                                                                    |
| `description`                                                                                                                                                                     | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The organisation description                                                                                                                                                      | Lorem Ipsum                                                                                                                                                                       |
| `industryName`                                                                                                                                                                    | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The organisation industry                                                                                                                                                         | Restaurant                                                                                                                                                                        |
| `industrySectors`                                                                                                                                                                 | [operations.ComCrmOrganisationSelfServiceResourceGetSingleIndustrySector](../../models/operations/com-crm-organisation-self-service-resource-get-single-industry-sector.md)[]     | :heavy_minus_sign:                                                                                                                                                                | Information about the organisation’s industry sectors                                                                                                                             |                                                                                                                                                                                   |
| `businessActivities`                                                                                                                                                              | [operations.ComCrmOrganisationSelfServiceResourceGetSingleBusinessActivity](../../models/operations/com-crm-organisation-self-service-resource-get-single-business-activity.md)[] | :heavy_minus_sign:                                                                                                                                                                | Information about the organisation’s business activities                                                                                                                          |                                                                                                                                                                                   |
| `addresses`                                                                                                                                                                       | [operations.ComCrmOrganisationSelfServiceResourceGetSingleAddress](../../models/operations/com-crm-organisation-self-service-resource-get-single-address.md)[]                    | :heavy_minus_sign:                                                                                                                                                                | Information about the organisation’s locations                                                                                                                                    |                                                                                                                                                                                   |
| `creatives`                                                                                                                                                                       | [operations.ComCrmOrganisationSelfServiceResourceGetSingleCreative](../../models/operations/com-crm-organisation-self-service-resource-get-single-creative.md)[]                  | :heavy_minus_sign:                                                                                                                                                                | Information about the organisation’s creatives                                                                                                                                    |                                                                                                                                                                                   |
| `tags`                                                                                                                                                                            | [operations.ComCrmOrganisationSelfServiceResourceGetSingleTag](../../models/operations/com-crm-organisation-self-service-resource-get-single-tag.md)[]                            | :heavy_minus_sign:                                                                                                                                                                | The tags of the organisation                                                                                                                                                      | [<br/>{<br/>"name": "Accounting"<br/>}<br/>]                                                                                                                                      |
| `contactInfo`                                                                                                                                                                     | [operations.ComCrmOrganisationSelfServiceResourceGetSingleContactInfo](../../models/operations/com-crm-organisation-self-service-resource-get-single-contact-info.md)[]           | :heavy_minus_sign:                                                                                                                                                                | Information about the organisation’s contact details                                                                                                                              |                                                                                                                                                                                   |
| `operationDetails`                                                                                                                                                                | [operations.ComCrmOrganisationSelfServiceResourceGetSingleOperationDetails](../../models/operations/com-crm-organisation-self-service-resource-get-single-operation-details.md)   | :heavy_minus_sign:                                                                                                                                                                | Defines the operation details of the organisation                                                                                                                                 |                                                                                                                                                                                   |
| `contactRegistry`                                                                                                                                                                 | [operations.ComCrmOrganisationSelfServiceResourceGetSingleContactRegistry](../../models/operations/com-crm-organisation-self-service-resource-get-single-contact-registry.md)     | :heavy_minus_sign:                                                                                                                                                                | Defines whether the organisation supports contact registry                                                                                                                        | true                                                                                                                                                                              |
| `customFields`                                                                                                                                                                    | [operations.ComCrmOrganisationSelfServiceResourceGetSingleCustomField](../../models/operations/com-crm-organisation-self-service-resource-get-single-custom-field.md)[]           | :heavy_minus_sign:                                                                                                                                                                | The organisations custom fields                                                                                                                                                   |                                                                                                                                                                                   |
| `orderCatalogs`                                                                                                                                                                   | [operations.ComCrmOrganisationSelfServiceResourceGetSingleOrderCatalog](../../models/operations/com-crm-organisation-self-service-resource-get-single-order-catalog.md)[]         | :heavy_minus_sign:                                                                                                                                                                | Information about the organisation’s order catalogs                                                                                                                               |                                                                                                                                                                                   |
| `wifiSites`                                                                                                                                                                       | [operations.ComCrmOrganisationSelfServiceResourceGetSingleWifiSite](../../models/operations/com-crm-organisation-self-service-resource-get-single-wifi-site.md)[]                 | :heavy_minus_sign:                                                                                                                                                                | A list of WiFi Sites that are related to the organisation                                                                                                                         |                                                                                                                                                                                   |