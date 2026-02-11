# ComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslationsResponse

OK

## Example Usage

```typescript
import {
  ComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslationsResponse,
} from "crmcom/models/operations";

let value:
  ComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslationsResponse =
    {
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
    };
```

## Fields

| Field                                                                                                                                                                                                                                  | Type                                                                                                                                                                                                                                   | Required                                                                                                                                                                                                                               | Description                                                                                                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `embeddedLinks`                                                                                                                                                                                                                        | [operations.ComCrmApplicationSelfServiceResourceGetApplicationEmbeddedLinksTranslationsEmbeddedLink](../../models/operations/com-crm-application-self-service-resource-get-application-embedded-links-translations-embedded-link.md)[] | :heavy_minus_sign:                                                                                                                                                                                                                     | Define links for embedded browser in front-end systems                                                                                                                                                                                 |