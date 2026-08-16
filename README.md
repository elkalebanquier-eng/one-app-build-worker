# One App Build Worker

Ce dépôt public ne contient que la définition du **moteur de compilation**. Il ne reçoit pas, ne versionne pas et ne publie jamais le code ZIP importé par les utilisateurs. Lors d’un build, One App fournit une URL temporaire vers l’archive ; la machine de compilation télécharge le ZIP, fabrique l’APK, puis détruit son espace de travail à la fin de l’exécution.

Chaque build dispose d’une machine GitHub hébergée, éphémère, sans secret One App, sans droit d’écriture sur le dépôt et avec une limite de 35 minutes. L’APK est remis sous forme d’artefact temporaire, conservé un seul jour. GitHub indique que les machines standards hébergées restent gratuites dans les dépôts publics ; la conservation des fichiers reste toutefois limitée, afin d’éviter une croissance non maîtrisée du stockage.[1]

Le moteur accepte les projets Expo/React Native, les projets Android conventionnels avec un module `app` et les sites HTML statiques. Un projet HTML est encapsulé dans une application Android distincte ; cela ne modifie pas l’implémentation native de One App.

## Référence

[1] [GitHub Docs — Billing for GitHub Actions](https://docs.github.com/billing/managing-billing-for-github-actions/about-billing-for-github-actions)
