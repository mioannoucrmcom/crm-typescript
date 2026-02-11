# ComCrmServiceRequestSelfServiceResourceCreateAddress

Address information for the service request

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceCreateAddress } from "crm/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceCreateAddress = {
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
};
```

## Fields

| Field                                                | Type                                                 | Required                                             | Description                                          | Example                                              |
| ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| `id`                                                 | *string*                                             | :heavy_minus_sign:                                   | The entity identifier                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                 |
| `other`                                              | [operations.Other](../../models/operations/other.md) | :heavy_minus_sign:                                   | Details about the address                            |                                                      |