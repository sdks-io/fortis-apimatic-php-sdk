
# Device 1

*This model accepts additional fields of type array.*

## Structure

`Device1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `deviceBindingStatus` | [`?string(DeviceBindingStatus)`](../../doc/models/device-binding-status.md) | Optional | - | getDeviceBindingStatus(): ?string | setDeviceBindingStatus(?string deviceBindingStatus): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "device_binding_status": "01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

