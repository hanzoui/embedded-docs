El cargador QuadrupleCLIP es uno de los nodos centrales de Hanzo Studio, que se agregó por primera vez para el soporte de modelos de la versión HiDream I1. Si notas que falta este nodo, intenta actualizar Hanzo Studio a la última versión para garantizar el soporte del nodo.

Requiere 4 modelos CLIP, que corresponden a los parámetros `clip_name1`, `clip_name2`, `clip_name3` y `clip_name4`, y proporcionará una salida de modelo CLIP para su uso en nodos posteriores.

Este nodo detectará los modelos ubicados en la carpeta `Hanzo Studio/models/text_encoders`,
y también leerá los modelos de las rutas adicionales configuradas en el archivo extra_model_paths.yaml.
A veces, después de agregar modelos, es posible que necesites **recargar la interfaz de Hanzo Studio** para que pueda leer los archivos de modelo en la carpeta correspondiente.
