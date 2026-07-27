# ☁️ Projet : Serveur pfSense sur Ubuntu (VM VirtualBox)

Ce projet explique comment installer et configurer un pare-feu **pfSense** dans une machine virtuelle **VirtualBox**.

Tu apprendras à installer pfSense, configurer les interfaces réseau, mettre en place le DHCP, les règles de pare-feu, le NAT et tester le bon fonctionnement du réseau.

---

# 🎯 Objectifs du projet

- Installer pfSense dans VirtualBox
- Configurer les interfaces WAN et LAN
- Configurer le serveur DHCP
- Créer des règles de pare-feu
- Comprendre le fonctionnement du NAT
- Tester la connectivité réseau
- Sécuriser un réseau local

---

# 💻 1. Téléchargement de pfSense

Télécharge l'image ISO depuis le site officiel :

https://www.pfsense.org/download/

---

# 🖥️ 2. Création de la machine virtuelle

Créer une nouvelle machine virtuelle.

**Configuration recommandée :**

- Type : BSD
- Version : FreeBSD (64 bits)
- Mémoire : 2 Go
- Processeurs : 2 cœurs
- Disque : 20 Go

Configurer deux cartes réseau :

- Carte 1 : NAT
- Carte 2 : Réseau interne

---

# 💿 3. Installation de pfSense

- Démarrer la VM
- Choisir Install
- Conserver les options par défaut
- Redémarrer la machine
- Retirer l'ISO

---

# 🌐 4. Configuration des interfaces

Attribuer les interfaces :

- WAN
- LAN

Configurer une adresse IP sur le LAN.

Exemple :

192.168.1.1/24

---

# 🌍 5. Accès à l'interface Web

Depuis une machine cliente :

https://192.168.1.1

Identifiants par défaut :

Utilisateur :

admin

Mot de passe :

pfsense

---

# ⚙️ 6. Configuration initiale

Configurer :

- Nom du pare-feu
- DNS
- Fuseau horaire
- Mot de passe administrateur

---

# 📡 7. Configuration du DHCP

Activer le serveur DHCP sur le réseau LAN.

Exemple :

192.168.1.100

à

192.168.1.200

---

# 🔥 8. Configuration des règles du pare-feu

Créer les règles nécessaires :

- Autoriser le LAN vers Internet
- Bloquer les connexions entrantes non autorisées
- Vérifier les règles par défaut

---

# 🌍 9. Vérification du NAT

Vérifier que le mode NAT est configuré en :

Automatic Outbound NAT

---

# 🧪 10. Tests

Tester :

- Ping vers Internet
- Résolution DNS
- Navigation Web

---

# 📚 Ressources

- Documentation officielle pfSense
- Documentation VirtualBox
