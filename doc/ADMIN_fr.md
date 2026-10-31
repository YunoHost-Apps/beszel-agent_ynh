## Configurer l'agent

Si vous avez manqué les informations de post-installation : votre agent Beszel écoute sur le port __PORT__.

La fenêtre `+ Add System` de Beszel devrait encore être ouverte. Saisissez-y ce port à la place du port par défaut `45876`, renseignez le nom, le domaine ou l'adresse IP du serveur à surveiller, puis cliquez sur `Add System`.

Si vous avez fermé cette fenêtre, il faut désinstaller puis réinstaller l'agent : le jeton est régénéré à chaque lancement de la procédure Add System.

## Configuration supplémentaire

L'agent surveille déjà l'essentiel sans réglage, mais vous pouvez compléter sa configuration à la main dans son fichier d'environnement.

Ajoutez vos ajustements dans `__DATA_DIR__/.env.local`, puis pensez à redémarrer le service `__APP__`.

### Disques supplémentaires

Pour utiliser `EXTRA_FILESYSTEMS`, voir la documentation officielle : <https://beszel.dev/guide/additional-disks#binary-agent>

### Surveillance du GPU

La documentation officielle (<https://beszel.dev/guide/gpu#gpu-monitoring>) décrit la configuration à prévoir pour que l'agent surveille votre GPU ; elle varie surtout selon la marque.
