> Esta documentación fue generada por IA. Si encuentra algún error o tiene sugerencias de mejora, ¡no dude en contribuir! [Editar en GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/LoadTrainingDataset/es.md)

Este nodo carga un conjunto de datos de entrenamiento codificado que ha sido previamente guardado en disco. Busca y lee todos los archivos de fragmentos de datos desde una carpeta específica dentro del directorio de salida de Hanzo Studio, y luego devuelve los vectores latentes combinados y los datos de condicionamiento para su uso en flujos de trabajo de entrenamiento.

## Entradas

| Parámetro | Tipo de Dato | Obligatorio | Rango | Descripción |
|-----------|-----------|----------|-------|-------------|
| `folder_name` | STRING | No | N/A | Nombre de la carpeta que contiene el conjunto de datos guardado, ubicada dentro del directorio de salida de Hanzo Studio (por defecto: "training_dataset"). |

## Salidas

| Nombre de Salida | Tipo de Dato | Descripción |
|-------------|-----------|-------------|
| `latents` | LATENT | Una lista de diccionarios latentes, donde cada diccionario contiene una clave `"samples"` con un tensor. |
| `conditioning` | CONDITIONING | Una lista de listas de condicionamiento, donde cada lista interna contiene datos de condicionamiento para una muestra correspondiente. |