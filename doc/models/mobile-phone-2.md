
# Mobile Phone 2

*This model accepts additional fields of type array.*

## Structure

`MobilePhone2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `cc` | `?string` | Optional | Country Code of the phone<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `3` | getCc(): ?string | setCc(?string cc): void |
| `subscriber` | `?string` | Optional | Subscriber section of the number<br><br>**Constraints**: *Maximum Length*: `15` | getSubscriber(): ?string | setSubscriber(?string subscriber): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "cc": "1",
  "subscriber": "5555555",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

