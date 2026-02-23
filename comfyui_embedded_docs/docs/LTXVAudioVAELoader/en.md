> This documentation was AI-generated. If you find any errors or have suggestions for improvement, please feel free to contribute! [Edit on GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/LTXVAudioVAELoader/en.md)

The LTXV Audio VAE Loader node loads a pre-trained Audio Variational Autoencoder (VAE) model from a checkpoint file. It reads the specified checkpoint, loads its weights and metadata, and prepares the model for use in audio generation or processing workflows within Hanzo Studio.

## Inputs

| Parameter | Data Type | Required | Range | Description |
|-----------|-----------|----------|-------|-------------|
| `ckpt_name` | STRING | Yes | All files in the `checkpoints` folder.<br>*Example: `"audio_vae.safetensors"`* | Audio VAE checkpoint to load. This is a dropdown list populated with all the files found in your Hanzo Studio `checkpoints` directory. |

## Outputs

| Output Name | Data Type | Description |
|-------------|-----------|-------------|
| `Audio VAE` | VAE | The loaded Audio Variational Autoencoder model, ready to be connected to other audio processing nodes. |