> Cette documentation a été générée par IA. Si vous trouvez des erreurs ou avez des suggestions d'amélioration, n'hésitez pas à contribuer ! [Modifier sur GitHub](https://github.com/hanzoui/embedded-docs/blob/main/hanzo_studio_embedded_docs/docs/LoadTrainingDataset/fr.md)

Ce nœud charge un jeu de données d'entraînement encodé précédemment enregistré sur le disque. Il recherche et lit tous les fichiers de fragments de données (shards) à partir d'un dossier spécifié dans le répertoire de sortie de Hanzo Studio, puis renvoie les vecteurs latents combinés et les données de conditionnement pour une utilisation dans les flux de travail d'entraînement.

## Entrées

| Paramètre | Type de données | Requis | Plage | Description |
|-----------|-----------|----------|-------|-------------|
| `folder_name` | STRING | Non | N/A | Nom du dossier contenant le jeu de données enregistré, situé à l'intérieur du répertoire de sortie de Hanzo Studio (par défaut : "training_dataset"). |

## Sorties

| Nom de la sortie | Type de données | Description |
|-------------|-----------|-------------|
| `latents` | LATENT | Une liste de dictionnaires latents, où chaque dictionnaire contient une clé `"samples"` avec un tenseur. |
| `conditioning` | CONDITIONING | Une liste de listes de conditionnement, où chaque liste interne contient les données de conditionnement pour un échantillon correspondant. |