# Ansible Mediahub

## Workflow de création de vm Mediahub

- Récupération des addresses ip disponibles dans les subnet nécessaires
- Creation de la vm de base (methode Proxmox/Clone VM)
- En fonction du type de VM mediahub, on modifie les ressources allouées à la VM (méthode Proxmox/config VM)
- Creation des records dans Powerdns via l'API
- Deploiement des applis mediahubs-admin
- Configuration des instances et interfaces en fonction du type de Remote/EdgeIn/Internal/EdgeOut. Une instance peut avoir plusieurs types de fonctions
