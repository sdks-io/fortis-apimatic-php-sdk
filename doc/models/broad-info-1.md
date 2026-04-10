
# Broad Info 1

*This model accepts additional fields of type array.*

## Structure

`BroadInfo1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `category` | [`?string(Category)`](../../doc/models/category.md) | Optional | - | getCategory(): ?string | setCategory(?string category): void |
| `description` | `?string` | Optional | Information to be broadcasted to the recipients. Accepted value length is maximum 4000 characters. This field is optional.<br><br>**Constraints**: *Maximum Length*: `4000` | getDescription(): ?string | setDescription(?string description): void |
| `expireDate` | `?string` | Optional | The date after which the relevance of the broadcasted information (e.g., ceritifacte expiration dates) expires. The accepted value length is 8 characters. The accepted format is YYYYMMDD.<br><br>**Constraints**: *Maximum Length*: `8` | getExpireDate(): ?string | setExpireDate(?string expireDate): void |
| `severity` | [`?string(Severity)`](../../doc/models/severity.md) | Optional | - | getSeverity(): ?string | setSeverity(?string severity): void |
| `recipients` | [`?string(Recipients)`](../../doc/models/recipients.md) | Optional | - | getRecipients(): ?string | setRecipients(?string recipients): void |
| `source` | [`?string(Source)`](../../doc/models/source.md) | Optional | - | getSource(): ?string | setSource(?string source): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "category": "82",
  "description": "description6",
  "expire_date": "expire_date6",
  "severity": "03",
  "recipients": "01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

