> This documentation was AI-generated. If you find any errors or have suggestions for improvement, please feel free to contribute! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/ConvertStringToComboNode/en.md)

The Convert String to Combo node takes a text string as input and converts it into a Combo data type. This allows you to use a text value as a selection for other nodes that require a Combo input. It simply passes the string value through unchanged but changes its data type.

## Inputs

| Parameter | Data Type | Required | Range | Description |
|-----------|-----------|----------|-------|-------------|
| `string` | STRING | Yes | N/A | The text string to be converted into a Combo type. |

## Outputs

| Output Name | Data Type | Description |
|-------------|-----------|-------------|
| `output` | COMBO | The input string, now formatted as a Combo data type. |