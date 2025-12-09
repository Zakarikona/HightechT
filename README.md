🛡️ Cyber Security Lab — TheHive, Cortex & MISP (Dockerized SOC Stack)
📄 Présentation du projet
Ce projet fait partie de mon Projet de Fin d’Études (PFE) en cybersécurité. L’objectif principal est de concevoir, déployer et intégrer une stack SOC open-source fonctionnelle comprenant :

TheHive : Plateforme de gestion et d’investigation des incidents.

Cortex : Moteur d’analyse et d’automatisation de réponses aux incidents.

MISP (Malware Information Sharing Platform) : Plateforme de partage d’indicateurs de compromission (IoC).

La stack est entièrement conteneurisée avec Docker, permettant une installation rapide, reproductible et modulable. Ce laboratoire vise à fournir un environnement pratique pour la simulation d’incidents, la corrélation de logs et l’analyse automatisée de menaces.

🎯 Objectifs pédagogiques et techniques

Maîtriser le déploiement de services SOC open-source via Docker / Docker Compose.

Comprendre l’intégration entre TheHive, Cortex et MISP pour un workflow SOC complet.

Créer un environnement de test réaliste pour l’analyse d’incidents et l’investigation cyber.

Fournir une base prête à l’emploi pour des démonstrations professionnelles ou académiques.

🔗 Documentation & Références

Guides et tutoriels utilisés pour construire le laboratoire :

Installation TheHive + Cortex + MISP avec Docker Compose

Intégration Cortex & MISP avec TheHive dans un SOC

🐳 Déploiement avec Docker Compose

Le fichier docker-compose.yml fourni permet de lancer l’ensemble de la stack :

git clone <repo-url>
cd cyber-security-lab
docker compose up -d


Accès aux services via navigateur ou API locale.

Configuration initiale prête à l’emploi pour tests et démonstrations.

💿 VirtualBox — VM préconfigurée

Pour ceux qui souhaitent tester la stack sans configuration manuelle, une VM Ubuntu 22.04 LTS est disponible :

👉 Télécharger la VM (.ova)

🔑 Informations de connexion
Service	Adresse / Login	Mot de passe
VM Ubuntu 22.04 (SSH)	10.200.200.253 – labuser	lab123
Cortex Admin	labuser	lab123
MISP Admin	admin@admin.test	admin
TheHive Default Admin	admin@thehive.local	secret
🖥️ Architecture SOC (Résumé)

MISP collecte et partage les IoC.

TheHive reçoit les alertes et organise les investigations.

Cortex automatise les analyses via des jobs sur les alertes de TheHive.

Intégration complète pour un SOC opérationnel, prêt pour la simulation d’incidents et la formation.

🏆 Résultats attendus

Déploiement d’un SOC open-source fonctionnel sur VM ou Docker.

Accès aux fonctionnalités de corrélation d’incidents et d’analyse automatisée.

Expérience pratique dans la gestion d’incidents cyber et l’utilisation d’outils SOC.

📌 Informations complémentaires

 Builder : Zakaria

Projet réalisé dans le cadre du Projet de Fin d’Études (PFE) – Cybersécurité

⚡ Conseils pour l’utilisation

Lancer la VM ou Docker Compose pour un environnement prêt à l’emploi.

Se connecter à TheHive et Cortex pour explorer la gestion d’incidents.

Tester l’intégration avec MISP pour enrichir les alertes et les analyses.
