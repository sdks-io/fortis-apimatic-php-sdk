
# Sms Blacklist

Sms Blacklist Information on `expand`

*This model accepts additional fields of type array.*

## Structure

`SmsBlacklist`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `id` | `?string` | Optional | Blacklist ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `isBlacklisted` | `?bool` | Optional | isBlacklisted | getIsBlacklisted(): ?bool | setIsBlacklisted(?bool isBlacklisted): void |
| `detail` | `?bool` | Optional | Contact Id | getDetail(): ?bool | setDetail(?bool detail): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "isBlacklisted": true,
  "detail": true,
  "created_ts": 1422040992,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

