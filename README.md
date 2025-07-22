# Azure-VM-Terraform-CI-CD

🚀 Projet inspiré de mon stage immersif Azure ☁️  
Automatisation du déploiement d’une machine virtuelle Linux sur Azure avec Terraform ⚙️,  
accompagnée d’une pipeline CI/CD GitHub Actions 🔁 pour valider la configuration.

---

## 📋 Contexte

Ce projet a été réalisé dans le cadre d’un stage immersif de 3 jours portant sur le déploiement Cloud Azure et la culture DevOps.  
Il vise à mettre en pratique les notions d’Infrastructure as Code (IaC) et de pipeline CI/CD observées sur le terrain.

---

## ⚙️ Fonctionnalités

- Déploiement automatisé d’une VM Linux sur Azure via Terraform
- Configuration modulaire avec variables Terraform
- Pipeline GitHub Actions qui vérifie formatage, initialisation, validation et plan Terraform à chaque push
- Documentation claire pour faciliter la prise en main

---

## 🚀 Prérequis

- Compte Azure actif avec droits suffisants pour créer ressources
- [Azure CLI](https://learn.microsoft.com/fr-fr/cli/azure/install-azure-cli) installé et configuré (`az login`)
- [Terraform](https://www.terraform.io/downloads) installé
- Clé SSH publique valide (ex. `~/.ssh/id_rsa.pub`)

---

## 🔧 Utilisation rapide

1. Cloner le dépôt :

git clone https://github.com/loicpgs/Azure-VM-Terraform-CI-CD.git
cd Azure-VM-Terraform-CI-CD

2. Vérifier et modifier si besoin le fichier variables.tf (notamment la clé SSH)

3. Initialiser Terraform :

terraform init

4. Vérifier le plan de déploiement :

terraform plan

5. Appliquer le déploiement :

terraform apply

⚙️ Pipeline CI/CD GitHub Actions

*Le pipeline se déclenche à chaque push sur la branche main et exécute :

*terraform fmt -check : vérifie la mise en forme des fichiers Terraform

*terraform init : initialise Terraform

*terraform validate : valide la configuration Terraform

*terraform plan : génère un plan de déploiement

📚 Ressources utiles

*Documentation Terraform Azure

*GitHub Actions

*Azure CLI

*Tutoriel Terraform Azure (Microsoft Learn)

✍️ Auteur

Loïc PAGES — Stagiaire TSSR — Juillet 2025

Licence:
M.I.T

