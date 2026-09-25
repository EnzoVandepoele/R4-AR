# Visualiseur 4L

Page statique qui affiche le modèle `4Llowpoly.glb` avec
[model-viewer](https://modelviewer.dev/) : orbite, zoom, rotation auto,
réglages d'éclairage, et mode AR sur mobile (`.usdz` sur iOS).

Aucun serveur n'est nécessaire : tout est statique.

## Aperçu local

Le chargement du `.glb` est bloqué en `file://`, il faut passer par HTTP :

    python -m http.server 8777

puis ouvrir <http://localhost:8777>.
