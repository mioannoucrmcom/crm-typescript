# AdvancedSettings

JSON scripts contaning specific mapping of existing settings to particular elements of the app. Used in special circumstances to allow fine tuning the app without rebuilding it. This is maintatined solely by front-end integrations and is not visible on the back-end user interface.

## Example Usage

```typescript
import { AdvancedSettings } from "crm/models/operations";

let value: AdvancedSettings = {};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `colours`                                                                                                        | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | JSON script contaning specific mapping of existing colour settings to particular elements of the app             |
| `layoutComponents`                                                                                               | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | JSON script contaning specific mapping of existing layout & component settings to particular elements of the app |