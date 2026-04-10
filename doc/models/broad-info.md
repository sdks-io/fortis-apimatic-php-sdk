
# Broad Info

Until EMV 3DS 2.2.0:

Unstructured information sent between the 3DS Server, the DS and the ACS.

This field is not required to be filled by the Requestor and the requirements for the presence of this field are DS specific.

Starting from EMV 3DS 2.3.1:

Structured information sent between the 3DS Server, the DS and the ACS. 2.3.1 structure is defined below. Accepted value length is maximum 4096 characters. This field is optional.

*This model accepts additional fields of type array.*

## Structure

`BroadInfo`

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
  "category": "98",
  "description": "description2",
  "expire_date": "expire_date0",
  "severity": "03",
  "recipients": "01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

