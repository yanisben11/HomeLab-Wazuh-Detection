# 🛡️ Projet Home Lab : Détection d'intrusions avec Wazuh SIEM

**Description du projet**
Mise en place d'une infrastructure de sécurité (SIEM) complète pour surveiller un réseau domestique, détecter des vulnérabilités et analyser des attaques en temps réel. Ce projet simule un environnement d'entreprise (SOC) à petite échelle.

## 🏗️ Architecture Technique (VMware)
* **Serveur SIEM :** Ubuntu Server hébergeant la solution **Wazuh** (Manager & Dashboard).
* **Machine Cible (Endpoint) :** Windows 10 Pro avec l'agent Wazuh installé.
    * Service surveillé : Serveur Web Apache (XAMPP).
    * Configuration spécifique : Édition du fichier `ossec.conf` pour l'ingestion des logs Apache.
* **Machine Attaquante :** Kali Linux (pour les tests de pénétration).

## ⚙️ Scénario de Test & Réalisations
1.  **Cartographie Réseau :** Utilisation de **Nmap** pour scanner les ports ouverts et valider les règles de pare-feu.
2.  **Simulation d'Attaque :** Lancement d'un scan de vulnérabilités web via **Nikto**.
3.  **Détection & Réponse :**
    * Configuration de règles personnalisées sur l'agent Wazuh.
    * Détection réussie des signatures d'attaque Nikto.
    * Génération d'alertes de sécurité (Rule ID 31101 - Web server 400 error code) dans le dashboard.

## 🚀 Compétences Validées
- [x] Administration Système Linux & Windows
- [x] Analyse de logs et corrélation d'événements (SIEM)
- [x] Protocoles Réseaux (TCP/IP, HTTP)
- [x] Gestion de vulnérabilités

---
*Projet réalisé par Yanis Benchabane - Janvier 2026*
