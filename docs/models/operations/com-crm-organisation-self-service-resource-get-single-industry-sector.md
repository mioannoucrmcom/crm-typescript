# ComCrmOrganisationSelfServiceResourceGetSingleIndustrySector

## Example Usage

```typescript
import { ComCrmOrganisationSelfServiceResourceGetSingleIndustrySector } from "crm/models/operations";

let value: ComCrmOrganisationSelfServiceResourceGetSingleIndustrySector = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Bar",
  relatedIndustries: [
    {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                           | Type                                                                                                                                                                            | Required                                                                                                                                                                        | Description                                                                                                                                                                     | Example                                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                            | *string*                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                              | The entity identifier                                                                                                                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                            |
| `name`                                                                                                                                                                          | *string*                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                              | The sub-industry name                                                                                                                                                           | Bar                                                                                                                                                                             |
| `relatedIndustries`                                                                                                                                                             | [operations.ComCrmOrganisationSelfServiceResourceGetSingleRelatedIndustry](../../models/operations/com-crm-organisation-self-service-resource-get-single-related-industry.md)[] | :heavy_minus_sign:                                                                                                                                                              | The related industries                                                                                                                                                          |                                                                                                                                                                                 |