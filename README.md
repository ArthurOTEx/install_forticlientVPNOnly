# Script d'Installation Automatique FortiClient VPN-Only

Ce dépôt contient un script Bash simple et efficace permettant d'automatiser le téléchargement et l'installation de **FortiClient VPN-Only** (version 7.4.3.1736) pour les architectures Linux en 64 bits (`amd64`).

Ce script est particulièrement utile pour déployer rapidement le client VPN de Fortinet sur des distributions basées sur Debian/Ubuntu sans avoir à effectuer les commandes manuellement.

## 🚀 Fonctionnalités

Le script exécute les actions suivantes en toute autonomie :
1. **Nettoyage** : Supprime les éventuels anciens fichiers d'installation résiduels de FortiClient présents dans le dossier temporaire `/tmp/`.
2. **Téléchargement sécurisé** : Télécharge le paquet officiel `.deb` de FortiClient VPN-Only directement depuis les serveurs de Fortinet (`filestore.fortinet.com`) avec une barre de progression.
3. **Installation** : Installe le paquet téléchargé et gère automatiquement la configuration ainsi que les dépendances nécessaires via `apt`.

## 📋 Prérequis

* Un système d'exploitation basé sur **Debian** ou **Ubuntu** (en architecture 64-bit / amd64).
* Une connexion Internet active.
* Les droits **root** ou l'accès à `sudo` pour l'installation du paquet.

## 🛠️ Téléchargement et Exécution

Vous avez deux possibilités pour récupérer et exécuter ce script : en clonant le dépôt ou en téléchargeant directement le fichier.

### Méthode 1 : Cloner le dépôt

```bash
git clone [https://raw.githubusercontent.com/ArthurOTEx/install_forticlientVPNOnly/refs/heads/main/intall_forticlientVPNOnly.sh](https://raw.githubusercontent.com/ArthurOTEx/install_forticlientVPNOnly/refs/heads/main/intall_forticlientVPNOnly.sh)
cd intall_forticlientVPNOnly
chmod +x intall_forticlientVPNOnly.sh
sudo ./intall_forticlientVPNOnly.sh
```

### Méthode 2 : Téléchargement direct avec curl
```bash
curl -O [https://raw.githubusercontent.com/ArthurOTEx/install_forticlientVPNOnly/refs/heads/main/intall_forticlientVPNOnly.sh](https://raw.githubusercontent.com/ArthurOTEx/install_forticlientVPNOnly/refs/heads/main/intall_forticlientVPNOnly.sh)
chmod +x intall_forticlientVPNOnly.sh
sudo ./intall_forticlientVPNOnly.sh
```
