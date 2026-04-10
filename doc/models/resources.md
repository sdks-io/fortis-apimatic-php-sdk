
# Resources

Resource Information on `expand`

*This model accepts additional fields of type array.*

## Structure

`Resources`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `title` | `?string` | Optional | Resource Title<br><br>**Constraints**: *Maximum Length*: `64` | getTitle(): ?string | setTitle(?string title): void |
| `priv` | `?string` | Optional | Priv<br><br>**Constraints**: *Maximum Length*: `64` | getPriv(): ?string | setPriv(?string priv): void |
| `resourceName` | `?string` | Optional | Resource Name<br><br>**Constraints**: *Maximum Length*: `64` | getResourceName(): ?string | setResourceName(?string resourceName): void |
| `id` | `?int` | Optional | Resource ID | getId(): ?int | setId(?int id): void |
| `lastUsedDate` | `?int` | Optional | Last Used Date | getLastUsedDate(): ?int | setLastUsedDate(?int lastUsedDate): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `modifiedTs` | `?int` | Optional | Modified Time Stamp | getModifiedTs(): ?int | setModifiedTs(?int modifiedTs): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "title": "My terminal",
  "resource_name": "v2.addons.iframe.get",
  "id": 5693,
  "last_used_date": 1422040992,
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "priv": "priv0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

