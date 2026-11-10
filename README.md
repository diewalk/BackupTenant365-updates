# Backup Tenant 365 By Occigen : mises à jour

Ce dépôt public sert les mises à jour de Backup Tenant 365 aux serveurs des clients d'Occigen. Il suit le même principe que
MacCare-updates.

- **`flux.txt`** : le flux des versions, publié par GitHub Pages à l'adresse
  `https://diewalk.github.io/BackupTenant365-updates/flux.txt`.
  - Il est signé par Occigen (ECDSA P-256). Chaque serveur vérifie la signature avec la clé publique intégrée au programme : un flux modifié est refusé.
  - Pour chaque version, il donne les notes et, pour chaque système, l'installateur avec son empreinte SHA-256 et sa taille.
- **Releases** : les installateurs de chaque version.
  - `BackupTenant365-Setup-<version>-<système>` : utilisés par la mise à jour depuis la console.
  - `BackupTenant365-Installateur-Synology-<version>-<système>` : à lancer à la main pour un NAS Synology.

Ce dépôt ne contient aucun secret ni code source. Le code est dans le dépôt privé `diewalk/BackupTenant365`.

La publication se fait avec `tools/publier-mise-a-jour.ps1`, depuis ce dépôt privé.
