Ce nœud détecte automatiquement les modèles situés dans le dossier `HanzoStudio/models/clip_vision`, ainsi que tout chemin supplémentaire configuré dans le fichier `extra_model_paths.yaml`. Si vous ajoutez des modèles après avoir démarré Hanzo Studio, veuillez **rafraîchir l'interface Hanzo Studio** pour vous assurer que la liste des fichiers de modèles est à jour.

## Entrées

| Champ      | Data Type      | Description |
|------------|---------------|-------------|
| nom_clip   | COMBO[STRING]  | Affiche tous les fichiers de modèles compatibles dans le dossier `HanzoStudio/models/clip_vision`. |

## Sorties

| Champ        | Data Type    | Description |
|--------------|--------------|-------------|
| clip_vision  | CLIP_VISION  | Modèle CLIP Vision chargé, prêt à encoder des images ou à effectuer d'autres tâches liées à la vision. |
