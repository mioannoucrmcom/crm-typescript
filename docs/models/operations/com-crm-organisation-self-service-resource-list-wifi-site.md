# ComCrmOrganisationSelfServiceResourceListWifiSite

## Example Usage

```typescript
import { ComCrmOrganisationSelfServiceResourceListWifiSite } from "crmcom/models/operations";

let value: ComCrmOrganisationSelfServiceResourceListWifiSite = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  siteId: "88quh2m6",
  integration: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
};
```

## Fields

| Field                                                                                                                                                     | Type                                                                                                                                                      | Required                                                                                                                                                  | Description                                                                                                                                               | Example                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                      | *string*                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                        | The entity identifier                                                                                                                                     | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                      |
| `siteId`                                                                                                                                                  | *string*                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                        | The WiFi platform site id                                                                                                                                 | 88quh2m6                                                                                                                                                  |
| `integration`                                                                                                                                             | [operations.ComCrmOrganisationSelfServiceResourceListIntegration](../../models/operations/com-crm-organisation-self-service-resource-list-integration.md) | :heavy_minus_sign:                                                                                                                                        | TDetails about the integration of the WiFi Site                                                                                                           |                                                                                                                                                           |