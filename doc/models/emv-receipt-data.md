
# Emv Receipt Data

This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM

*This model accepts additional fields of type array.*

## Structure

`EmvReceiptData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `aid` | `?string` | Optional | This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM | getAid(): ?string | setAid(?string aid): void |
| `applab` | `?string` | Optional | This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM | getApplab(): ?string | setApplab(?string applab): void |
| `appn` | `?string` | Optional | This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM | getAppn(): ?string | setAppn(?string appn): void |
| `cvm` | `?string` | Optional | This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM | getCvm(): ?string | setCvm(?string cvm): void |
| `tsi` | `?string` | Optional | This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM | getTsi(): ?string | setTsi(?string tsi): void |
| `tvr` | `?string` | Optional | This field is a read only field. This field will only be populated for EMV transactions and will contain proper JSON formatted data with some or all of the following fields: TC,TVR,AID,TSI,ATC,APPLAB,APPN,CVM | getTvr(): ?string | setTvr(?string tvr): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "AID": "a0000000042203",
  "APPLAB": "US Maestro",
  "APPN": "US Maestro",
  "CVM": "Pin Verified",
  "TSI": "e800",
  "TVR": "0800008000",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

