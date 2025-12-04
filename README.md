# Unity Care Clinic – Backend (PHP 8.5 procédural + MySQLi)

##  Introduction

Ce projet représente la **première version du backend** de la plateforme **Unity Care Clinic**, développée en **PHP 8.5 procédural** et **MySQLi**.
Il a pour objectif de fournir une base solide permettant de gérer les différentes entités de la clinique, telles que les **patients**, **médecins** et **départements**, tout en offrant un **tableau de bord dynamique** pour visualiser les statistiques clés du système.

Cette version se concentre sur la simplicité, la lisibilité et une architecture facilement maintenable, adaptée à un premier déploiement.

---

##  Objectifs du Projet

* Construire un backend fonctionnel et structuré en PHP procédural.
* Permettre la gestion complète (CRUD) des entités principales.
* Proposer un tableau de bord dynamique avec statistiques et graphiques.
* Intégrer un système multilingue (i18n) basé sur des fichiers de langue.
* Fournir une documentation complète pour l’installation et l’utilisation.

---

##  Fonctionnalités Principales

### 1. **Gestion des Entités (CRUD)**

✔ Patients : ajout, modification, suppression, affichage
✔ Départements : création, mise à jour, suppression, listing
✔ Médecins : gestion complète + association avec un département
✔ Relations MySQL (clé étrangère : médecin → département)

---

### 2. **Tableau de Bord (Dashboard)**

Le dashboard présente des informations essentielles :

* Nombre total de médecins
* Nombre total de patients
* Nombre de départements
* Graphiques dynamiques (Chart.js)
* Répartition des entités

---

### 3. **Internationalisation (i18n)**

Le backend propose un système multilingue via :

* `/lang/fr.php`
* `/lang/en.php`
* `/lang/es.php`

L’administrateur peut changer la langue depuis l’interface.

---

### 4. **Bonus (Optionnel)**

* AJAX pour les opérations sans rechargement
* Modals pour une navigation plus fluide
* Graphiques avancés

---

##  Structure du Projet

```
/config
    db.php                  # Connexion MySQLi
/controllers
    patients.php
    doctors.php
    departments.php
/models
    patient_model.php
    doctor_model.php
    department_model.php
/views
    dashboard.php
    patients_list.php
    patient_form.php
/lang
    fr.php
    en.php
    es.php
/assets
    /css
    /js
index.php
README.md
```

---

##  Technologies Utilisées

* **PHP 8.5 (procédural)**
* **MySQL / MySQLi**
* **HTML5 / CSS3 / JS**
* **Chart.js** pour les graphiques
* **AJAX** (optionnel)

---

##  Installation & Configuration

### 1. **Prérequis**

* PHP ≥ 8.5
* MySQL ≥ 5.7
* Serveur local (Laragon, XAMPP, WAMP...)
* Navigateur moderne

---

### 2. **Installation**

1. Clonez le projet :

```bash
git clone https://github.com/USERNAME/unity-care-clinic-backend.git
```

2. Importez le fichier SQL :

* Ouvrez phpMyAdmin
* Créez une base de données : `clinic_db`
* Importez `clinic_db.sql`

3. Configurez la connexion MySQL dans :
   `/config/db.php`

```php
$connection = mysqli_connect("localhost", "root", "", "clinic_db");
```

4. Lancez le serveur local :

```
http://localhost/unity-care-clinic-backend/
```

---

##  Schémas du Projet

### ✔ ERD

Inclut : Patients, Doctors, Departments, relations clé étrangère.
*(Voir dossier /docs)*

### ✔ UML – Cas d’utilisation

* Gestion des patients
* Gestion des médecins
* Gestion des départements
* Dashboard

---

##  Déploiement (Optionnel)

Vous pouvez héberger le projet sur :

* InfinityFree
* 000WebHost
* Hostinger
* Un VPS Linux

---

##  Livrables (déjà inclus dans le dépôt)

* Code PHP complet
* Fichier SQL
* README
* ERD + UML
* Rapport du livrable
* Lien Jira (planification)

---

##  Licence

Projet réalisé pour un objectif académique (YouCode) dans le cadre du développement backend en PHP procédural.

---

##  Auteur

**Nom :** Ridouane El habib
**GitHub :** [https://github.com/redel-byte](https://github.com/redel-byte)

---

##  Contact

Pour toute question :
 *[alhabibridouane@gmail.com](alhabibrioduane@gmail.com)*

---

