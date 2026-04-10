
# Status 5

*This model accepts additional fields of type array.*

## Structure

`Status5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `responseCode` | `?string` | Optional | Response code for API response.<br><br>**Constraints**: *Maximum Length*: `20` | getResponseCode(): ?string | setResponseCode(?string responseCode): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response_code": "Received",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

