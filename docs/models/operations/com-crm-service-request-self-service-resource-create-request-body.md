# ComCrmServiceRequestSelfServiceResourceCreateRequestBody

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceCreateRequestBody } from "crm/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceCreateRequestBody = {
  description: "I have a query about the potholes in Nicosia Main Road",
  queueId: "6b888b83-b418-752f-604d-0653cf658811",
  address: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    other: {
      name: "Engomi office",
      isPrimary: true,
      addressLine1: "21 Elia Papakyriakou",
      addressLine2: "7 Stars Tower",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2415",
      countryCode: "CYP",
      lat: 35.157115,
      lon: 33.313719,
      googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
    },
  },
  categories: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    },
  ],
  customFields: [
    {
      key: "back_office",
      value: "0001-12345",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                 | Type                                                                                                                                                                  | Required                                                                                                                                                              | Description                                                                                                                                                           | Example                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `description`                                                                                                                                                         | *string*                                                                                                                                                              | :heavy_check_mark:                                                                                                                                                    | The service request description                                                                                                                                       | I have a query about the potholes in Nicosia Main Road                                                                                                                |
| `queueId`                                                                                                                                                             | *string*                                                                                                                                                              | :heavy_check_mark:                                                                                                                                                    | The queue identifier                                                                                                                                                  | 6b888b83-b418-752f-604d-0653cf658811                                                                                                                                  |
| `address`                                                                                                                                                             | [operations.ComCrmServiceRequestSelfServiceResourceCreateAddress](../../models/operations/com-crm-service-request-self-service-resource-create-address.md)            | :heavy_minus_sign:                                                                                                                                                    | Address information for the service request                                                                                                                           |                                                                                                                                                                       |
| `categories`                                                                                                                                                          | [operations.ComCrmServiceRequestSelfServiceResourceCreateCategory](../../models/operations/com-crm-service-request-self-service-resource-create-category.md)[]        | :heavy_minus_sign:                                                                                                                                                    | Default categories added to the service request based on queue definition                                                                                             |                                                                                                                                                                       |
| `customFields`                                                                                                                                                        | [operations.ComCrmServiceRequestSelfServiceResourceCreateCustomField](../../models/operations/com-crm-service-request-self-service-resource-create-custom-field.md)[] | :heavy_minus_sign:                                                                                                                                                    | Custom fields relevant to this service request                                                                                                                        |                                                                                                                                                                       |