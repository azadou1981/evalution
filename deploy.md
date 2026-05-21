# Rapport de déploiement - [TANZILLI Azad]

## Liens

- **Application en ligne :** [https://eval-az.osc-fr1.scalingo.io/]
- **Dépôt de code :** [https://github.com/azadou1981/evalution]

---

## Prérequis techniques

- **Langage :** PHP 
- **Framework :** Symfony 
- **Moteur de templates :** Twig 
- **Gestionnaire de dépendances :** Composer 
- **Plateforme de déploiement :** Scalingo 

---

## Fichier de configuration CI

### 1. Création de l'application sur Scalingo

1. Se connecter au [dashboard Scalingo](https://dashboard.scalingo.com/).
2. Cliquer sur **"Create a new application"**.
3. Nommer l'application : `eval-az`.

### 2. Liaison avec le dépôt GitHub

1. Dans l'onglet **Deploy** de l'application, choisir **GitHub** comme méthode de déploiement.
2. Sélectionner le dépôt `azadou1981/evalution`.

### 3. Configuration des variables d'environnement (si besoin)

Si le projet nécessite des variables spécifiques (ex: `APP_ENV=prod`), les ajouter dans l'onglet **Environment** du dashboard Scalingo.

### 4. Déploiement

**Déploiement manuel :**
- Se rendre dans l'onglet **Deploy** > **Manual deployment**.
- Sélectionner la branche `main` (ou `master`).
- Cliquer sur **Deploy**.

### 5. Vérification

- Attendre que le build se termine
- Une fois le statut **"Deployed"** affiché, ouvrir l'URL : https://eval-az.osc-fr1.scalingo.io/

---


