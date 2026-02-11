# FontEnum

The text font style that will be used by the application

## Example Usage

```typescript
import { FontEnum } from "crmcom/models/operations";

let value: FontEnum = "Georgia";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"San Francisco" | "Roboto" | "Helvetica" | "Open Sans" | "Poppins" | "Georgia" | "Gilroy" | Unrecognized<string>
```