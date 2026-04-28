# ExamENS - Exam Management System

## Description
ExamENS est une application web de gestion des examens développée avec Angular.  
Elle permet la gestion des étudiants, enseignants et administrateurs avec un système d’authentification basé sur les rôles.

Le projet utilise JSON Server comme API simulée et met en pratique les concepts de routing, guards, services, formulaires réactifs et architecture modulaire.

---

## Fonctionnalités

- Authentification des utilisateurs
- Gestion des rôles (Admin, Enseignant, Étudiant)
- Tableau de bord pour chaque rôle
- Gestion des examens (ajout, modification, suppression, affichage)
- Gestion des notes et résultats
- Formulaires réactifs
- Protection des routes avec guards
- Communication avec une API JSON Server

---

## Technologies utilisées

- Angular
- TypeScript
- HTML
- SCSS
- RxJS
- JSON Server

---

## Structure du projet

src/
 ├── app/
 │    ├── auth/
 │    ├── admin/
 │    ├── enseignant/
 │    ├── etudiant/
 │    ├── core/
 │    │    ├── services/
 │    │    ├── guards/
 │    │    ├── interceptors/
 │    ├── layout/
 │    ├── models/

---

## Installation

### Cloner le projet
git clone https://github.com/aatimade/examens-angular-app.git  
cd examens-angular-app  

### Installer les dépendances
npm install  

### Lancer le projet Angular
ng serve --open  

### Lancer JSON Server
json-server --watch db.json --port 3000  

---

## Comptes de test

Admin  
Email: admin@ens.ma  
Mot de passe: admin123  

Enseignant  
Email: m.alaoui@ens.ma  
Mot de passe: prof123  

Étudiant  
Email: youssef.idrissi@ens.ma  
Mot de passe: etud123  

---

## Flux d’authentification

1. L’utilisateur se connecte
2. Vérification des identifiants via JSON Server
3. Le rôle est stocké dans le navigateur
4. Redirection selon le rôle
5. Protection des routes avec guards

---

## Auteur

Projet réalisé par un étudiant en informatique

---

## Améliorations futures

- Authentification JWT
- Backend réel (Node.js ou Spring Boot)
- Interface responsive
- Tableau de bord avancé
- Mode sombre
