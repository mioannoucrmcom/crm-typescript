# Shortcuts

Defines the supported shortcuts features

## Example Usage

```typescript
import { Shortcuts } from "crm/models/operations";

let value: Shortcuts = {
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
            },
          ],
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                        | Type                                                         | Required                                                     | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `isSupported`                                                | *boolean*                                                    | :heavy_minus_sign:                                           | Are shortcuts enabled?                                       |
| `shortcuts`                                                  | [operations.Shortcut](../../models/operations/shortcut.md)[] | :heavy_minus_sign:                                           | Configured shortcuts                                         |