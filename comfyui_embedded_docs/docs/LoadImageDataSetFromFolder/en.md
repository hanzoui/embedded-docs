> This documentation was AI-generated. If you find any errors or have suggestions for improvement, please feel free to contribute! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/LoadImageDataSetFromFolder/en.md)

This node loads multiple images from a specified subfolder within Hanzo Studio's input directory. It scans the chosen folder for common image file types and returns them as a list, making it useful for batch processing or dataset preparation.

## Inputs

| Parameter | Data Type | Required | Range | Description |
|-----------|-----------|----------|-------|-------------|
| `folder` | STRING | Yes | *Multiple options available* | The folder to load images from. The options are the subfolders present in Hanzo Studio's main input directory. |

## Outputs

| Output Name | Data Type | Description |
|-------------|-----------|-------------|
| `images` | IMAGE | List of loaded images. The node loads all valid image files (PNG, JPG, JPEG, WEBP) found in the selected folder. |