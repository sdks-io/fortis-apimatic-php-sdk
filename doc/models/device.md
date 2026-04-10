
# Device

Contains device information.

Available for supporting EMV 3DS 2.3.1 and later versions.

*This model accepts additional fields of type array.*

## Structure

`Device`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `deviceBindingStatus` | [`?string(DeviceBindingStatus)`](../../doc/models/device-binding-status.md) | Optional | - | getDeviceBindingStatus(): ?string | setDeviceBindingStatus(?string deviceBindingStatus): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "device_binding_status": "38",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

