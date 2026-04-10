
# Ui Prefs

Ui Prefs

*This model accepts additional fields of type array.*

## Structure

`UiPrefs`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `entryPage` | `?string` | Optional | Ui Prefs Entry Page | getEntryPage(): ?string | setEntryPage(?string entryPage): void |
| `pageSize` | `?int` | Optional | Ui Prefs Page Size<br><br>**Constraints**: `>= 0`, `<= 99` | getPageSize(): ?int | setPageSize(?int pageSize): void |
| `reportExportType` | `?array` | Optional | - | getReportExportType(): ?array | setReportExportType(?array reportExportType): void |
| `processMethod` | `?array` | Optional | - | getProcessMethod(): ?array | setProcessMethod(?array processMethod): void |
| `defaultTerminal` | `?string` | Optional | Ui Prefs Default Termianl<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getDefaultTerminal(): ?string | setDefaultTerminal(?string defaultTerminal): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "entry_page": "dashboard",
  "page_size": 2,
  "default_terminal": "11e95f8ec39de8fbdb0a4f1a",
  "report_export_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "process_method": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

