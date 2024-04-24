# Ansible Playbook pour le déploiement de serveurs Nginx et MariaDB

Ce dépôt contient un playbook Ansible et un fichier d'inventaire YAML pour déployer les serveurs Nginx et MariaDB sur des machines Linux.

## Contenu du dépôt

- inventory.yml: Ce fichier d'inventaire YAML contient les informations sur les machines à gérer. Il définit deux groupes d'hôtes : "web_servers" pour les serveurs web et "db_servers" pour les serveurs de base de données.
- playbook.yml: Ce playbook Ansible contient les tâches nécessaires pour installer Nginx sur les serveurs web et MariaDB sur les serveurs de base de données.

## Utilisation

1. Assurez-vous d'avoir Ansible installé sur votre machine de contrôle.
2. Clonez ce dépôt sur votre machine locale :

``bash
git clone https://github.com/MrCelsus/Ansible_quests.git
``

3. Modifiez le fichier inventory.yml pour spécifier les adresses IP ou les noms d'hôtes de vos propres serveurs.
4. Exécutez le playbook Ansible avec la commande suivante :
``bash
ansible-playbook -i inventory.ini installation.yml
``

## Personnalisation

Vous pouvez personnaliser les tâches du playbook ou ajouter de nouvelles tâches en fonction de vos besoins spécifiques.
Vous pouvez également modifier l'inventaire pour inclure d'autres groupes d'hôtes ou des propriétés supplémentaires pour chaque hôte.

## Prérequis

Une machine de contrôle Ansible avec Ansible installé.
Des machines cibles accessibles via SSH et disposant d'un utilisateur avec des privilèges sudo.
Assurez-vous de bien mettre les adresses IP de VOS machines 
