# Visualiseur 4L

Page statique qui affiche le modèle `4Llowpoly.glb` avec
[model-viewer](https://modelviewer.dev/) : orbite, zoom, rotation auto,
réglages d'éclairage, et mode AR sur mobile (`.usdz` sur iOS).

## Publier sur GitHub Pages

1. Pousser le dossier sur un dépôt GitHub.
2. Settings > Pages > Source : `Deploy from a branch`, branche `main`, dossier `/ (root)`.
3. La page est servie sur `https://<utilisateur>.github.io/<depot>/`.

Aucun serveur n'est nécessaire : tout est statique.

## Aperçu local

Le chargement du `.glb` est bloqué en `file://`, il faut passer par HTTP :

    python -m http.server 8777

puis ouvrir <http://localhost:8777>.
